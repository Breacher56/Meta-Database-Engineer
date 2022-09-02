# End-of-Course Graded Assessment: Using Python

1. Python is an interpreted language. Which of the following statements correctly describes an interpreted language?
    - The source code is pre-built and compiled before running.
    - Python will save all code first prior to running. 
    - The source code is converted into bytecode that is then executed by the Python virtual machine.
    - Python needs to be built prior to it being run.
    ```
    Answer: The source code is converted into bytecode that is then executed by the Python virtual machine.
    Explanation: Unlike other programming languages Python does not need to be built or linked for the code to run.
    ```

2. Why is indentation important in Python?
    - The code will compile faster with indentation. 
    - Python used indentation to determine which code block starts and ends. 
    - It makes the code more readable. 
    - The code will be read in a sequential manner
    ```
    Answer: Python used indentation to determine which code block starts and ends.
    Explanation: Python does not use curly braces like other languages, so it leverages off indentation to determine where the code blocks start and end.
    ```

3. What will be the output of the following code?
    ```python
    names = ["Anna", "Natasha", "Mike"]
    names.insert(2, "Xi")
    print(names)
    ```
    - ["Anna", "Natasha", "Xi", "Mike"]
    - ["Anna", "Natasha", "Xi"]
    - ["Anna", "Xi", "Mike"]
    - ["Anna", "Natasha", 2, "Xi", "Mike"]
    ```
    Answer: ["Anna", "Natasha", "Xi", "Mike"]
    Explanation: The insert() function displaces the remaining list after inserting the element passed. 
    ```

4. What will be the output of the code below?
    ```python
    for x in range(1, 4):
        print(int((str((float(x))))))
    ```
    - 1 , 2
    - “one”, “two”
    - 1.0, 2.0
    - Will give an error
    ```
    Answer: Will give an error
    Explanation: The float will first convert into string and output such as <class 'float'> which cannot be converted into int. 
    ```

5. What will be the output of the following code:
    ```python
    sample_dict = {1: 'Coffee', 2: 'Tea', 3: 'Juice'}
    for x in sample_dict:
        print(x)
    ```
    - 1 
    
      2 
      
      3
    - 'Coffee', 'Tea', 'Juice'
    - {1 2 3}
    - (1, 'Coffee')

      (2, 'Tea')

      (3, 'Juice')
    ```
    Answer: 1 
            2 
            3
    Explanation: The default values printed from a dictionary are keys.
    ```

6. What will be the output of the recursive code below?
    ```python
    def recursion(num):
        print(num)
        next = num - 3
        if next > 1:
            recursion(next)

    recursion(11)
    ```
    - 2 5 8 11
    - 2 5 8
    - 8 5 2
    - 11 8 5 2
    ```
    Answer: 11 8 5 2
    Explanation: The values printed have difference of 3, but printed in opposite order. 
    ```

7. What will be the type of time complexity for the following piece of code:
    ```python
    def bigo(numbers):
        for i in numbers:
            print(numbers)

    bigo([1, 7, 13, 19])
    ```
    - Logarithmic Time
    - Linear Time
    - Quadratic Time
    - Constant Time
    ```
    Answer: Linear Time
    Explanation: The single for loop will have linear time depending on the size of the input sequence.
    ```

8. What will be the output of the code below:
    ```python
    str = 'Pomodoro'
    for l in str:
    if l == 'o':
        str = str.split()
        print(str, end=", ")
    ```
    - Will throw an error
    - ['P', 'm', 'd', 'o']
    - ['Pomodoro', 'modoro', 'doro', 'ro']
    - ['Pomodoro']
    ```
    Answer: Will throw an error
    Explanation: The first time split() function is used, the str variable will convert into a list over which split() cannot be used and will give an error. 
    ```

9. Find the output of the code below:
    ```python
    def d():
        color = "green"
        def e():
            nonlocal color
            color = "yellow"
        e()
        print("Color: " + color)
        color = "red"
    color = "blue"
    d()
    ```
    - blue
    - yellow
    - red
    - green
    ```
    Answer: yellow
    Explanation: The color variable will retain the value from the nonlocal variable from e()
    ```

10. Find the output of the code below:
    ```python
    num = 9
    class Car:
        num = 5
        bathrooms = 2

    def cost_evaluation(num):
        num = 10
        return num

    class Bike():
        num = 11

    cost_evaluation(num)
    car = Car()
    bike = Bike()
    car.num = 7
    Car.num = 2
    print(num)
    ```
    - 2
    - 10
    - 9
    - 5
    ```
    Answer: 9
    Explanation: The value of the global variable will remain unchanged. 
    ```

11. Which of the following is the correct implementation that will return True if there is a parent class P, with an object p and a sub-class called C, with an object c?
    - print(issubclass(P,C))
    - print(issubclass(p,C))
    - print(issubclass(C,P))
    - print(issubclass(C,c))
    ```
    Answer: print(issubclass(C,P))
    Explanation: It can be read as C is sub-class of P.
    ```

12. Django is a type of:
    - Asynchronous framework
    - Micro-framework
    - Full-stack framework
    ```
    Answer: Full-stack framework
    Explanation: Django is a Full-stack framework.
    ```

13. Which of the following is not true about Integration testing:
    - It is where the application is tested as a whole.
    - It combines unit tests.
    - Tests the flow of data from one component to another.
    - Primarily dealt by the tester.
    ```
    Answer: It is where the application is tested as a whole.
    Explanation: This is the case with system testing.
    ```

14. While using pytest for testing, it is necessary to run the file containing the main code before we can run the testing file containing our unit tests.
    - False
    - True
    ```
    Answer: False
    Explanation: The main file must be saved to keep it updated but it is not required to be executed. We have to import it into our testing file. 
    ```

15. What will be the output of the code below:
    ```python
    class A:
        def a(self):
            return "Function inside A"

    class B:
        def a(self):
            return "Function inside B"

    class C:
        pass

    class D(C, A, B):
        pass

    d = D()
    print(d.a())
    ```
    - No output
    - Function inside B
    - None of the above
    - Function inside A
    ```
    Answer: Function inside A
    Explanation: The class A comes before class B in terms of the parent classes of class D.
    ```