# To print or not to print

In this chapter we will focus on **branching** and we will learn a bit about **variables** and **Python** itself.


## Branching

Branching is one of the most basic concepts in programming.

It basically allows our program to **decide** what to do based on some **conditions**.

> If player presses W, his character moves up.
>
> If he doesn't, his character stays still.

Most programs include branching logic somewhere in them.

## If then

Try running **NameReview.py** in src.

Let's understand that file.

---

```python
1: name = input("Jak se jmenuješ?\n> ")
```

This line you already know. But let's talk about what's actually happening here.
- The `name` is a **variable**.
    > **Variables** hold data.
    
    > That data can be a **string** like in this case (a sequence of characters - ie. text)

    > But variable can also contain numbers, booleans, arrays, even entire pictures! (We will learn about variables later)
- The `input(...)` calls a **function** called input.
    > **Input** function accepts a string as an argument and returns a string.

    > It print's the text, and then waits for user input (Ended by Enter/new line). It then returns that input. 

    > We will also talk about functions later down the line.

- The equals sign (`=`) takes the result of **input** and assigns it to the `name` variable.

---

```python
if name == "Aleš":
    print("Tyjo, máš fakt hustý jméno.\n\n10/10")
```

This is were the program **branches**. It can go in two different directions based on user input:
1. When the variable is equal to something specific, the program will call the print function with reaction to that.
2. If it's not, the program will skip the print function and continue.

---

```python
if name == "Tomáš":
    print("No... mohlo by to být lepší, ale i mnohem mnohem horší.\n\n6/10")
```

Same thing here.

---

```python
if name != "Tomáš" and name != "Aleš":
    print("Hele sorry, ale řekni rodičům že ti dali jméno pro retarda.\n\n1/10")
```

The reason I put this last condition here is that if I didn't the program would just do nothing and end if your name is neither Aleš nor Tomáš.

Usually, this is not the way to go. It's ugly and clunky.

Your task is to learn about **elif** statement and use it inside **NameReviewButBetter.py** to create the same functionality but using shorter more readable code.
Hint: You will use something like
```
if ...:
elif ...:
else:
``` 

## Equals and Equals?

You might have noticed that sometimes there is one equal sign and sometimes two.

So what's the dfference between `=` and `==`?

It's simple.

`=` is assignment operator. It takes the value on the right and assigns it to the variable on the left.

`nice = 69`

`alsoNice = nice`

`==` is a comparison operator.

It returns `True` if the values on the left and on the right are the equivalent.

And it returns `False` otherwise.

`48 == 1` returns **False**

`48 == 2 * 24` returns **True**

`alsoNice == nice` returns **True**

## Python is weird little snake

The structure of the if-else statement in most programming languages looks something like this:

```csharp
if (ThisIsTrue())
{
    DoThis();
    AndThat();
}
else //Else is optional
{
    DoSomethingEntirelyDifferent();
}
```

But python doesn't use parenthesees for the condition and it doesn't use curly braces for the body of the if statement.

So how does python know **what belongs to the if statement** and what doesn't??

>The answer is **tabs** and **colons**!

The equivalent code in **python** looks like this:

```python
if thisIsTrue():
    doThis()
    andThat()
else:
    doSomethingDifferent()
```

In most languages **whitespaces** (such as a space or a tab) don't have any meaning at all.

In python **tabs are super important**. For instance:

```python
if isYoMommaUgly():
    printYoMommaJoke()
apologize()
moveOn()
```

This program has a bug in it.

If yor mom is ugly (ie. if isYoMommaUgly **function** returns **true**) the output of the program is okay.

- It insults your mom
- apologises
- moves on

But if the **condition** is not met (ie. isYoMommaUgly **function** returns **false**) The program apologises for insulting your mom without actually doing it...

You can try to fix this bug yourself in **YoMomma.py**.

> By the way. You **will** create this exact bug yourself in the future at least once. That's not only okay but a part of every python programmer's journey.

## Text Game engine

Now that you know **print**, **input** and **if-else** statements we can move to actually coding something interesting.

Your last task for this lesson is to create a text game.

My idea is something like Escaping a haunted house but you can do anything you like.

Here are the requirements:

- At least **4 different endings** (3 deaths and an escape?)
- You should use **inner if statements**.
  ```python
  #Example:
  if day == True: #Same as 'if day:'
    if timeOfDay == 'Morning':
        goToWork()
    elif timeOfDay == 'Afternoon':
        relax()
    else: #if it's not morning nor afternoon then it's evening
        brushTeeth()
  else: #if it's not day, then it's night
    sleep()
  ```
  **Remember to tab every line correctly!**
- The game must handle wrong inputs - ie. When I input something that is not part of the game, I should know about it and the game should handle it somehow.
  > (For now it can just output `Wrong input` and end. If you want though, you can learn about `while` statement and use it to give player infinite retries until he inputs something correct.)

## TODO
- [ ] Recreate NameReview using **elif** and **else** statements.
- [ ] Fix the bug in **YoMomma.py**
- [ ] Write a text game in **TextGameEngine/V1**
- [ ] Push changes to Github
