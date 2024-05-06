# Tutorial 10
Fikri Risyad Indratno</br>
2206031170</br>
Advanced Programming B</br>

---

## Reflection

![](images/img1.png)

The async function runs outside of the main function and the program won't for the async function to finish to continue its execution, causing `hey hey` to be printed before `howdy!` and `done!` even though `println!("hey hey")` was placed after `spawner.spawn`.