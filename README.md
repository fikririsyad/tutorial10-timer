# Tutorial 10
Fikri Risyad Indratno</br>
2206031170</br>
Advanced Programming B</br>

---

## Reflection

![](images/img1.png)

The async function runs outside of the main function and the program won't for the async function to finish to continue its execution, causing `hey hey` to be printed before `howdy!` and `done!` even though `println!("hey hey")` was placed after `spawner.spawn`.

![](images/img2.png)

From the image above, we can see that `done3!` was printed before `done2!`. This happened because the program runs concurrently, so the order of execution can be different and is up to the `executor`.

![](images/img3.png)

If we remove `drop(spawner)`, the program will not finish because the `executor` doesn't know that there are no more tasks, so it will wait for new tasks even though there are no more tasks, causing the program to never die.