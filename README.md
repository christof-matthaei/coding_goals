# coding_goals
general coding goals i try to achieve

# 1.Make your code as easy to reason about as you can

## Make the scope of the variable as small as you can

#### avoid global non-const variable
#### avoid raw-loops
- Use the STL-algorithm and customize them for easier use
- Write your own STL-like algorithms

#### avoid non-const shared_ptr

#### Exception 
Don't cripple your code with scopes
```
void foo()
{
  Data d;
  {
    Path p("/foo/file.txt")
    FileReader f(p);
    f.copy_to(d);
  }//f p scopes ands here
  //more stuff
}
```
Hint: If you can cripple the code in the above way, write a new function

## 1.2 Don't use true,false in function calls
