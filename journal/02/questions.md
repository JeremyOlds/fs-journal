# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > let and const

02. What is the definition of a function?

    > a block of code that can be manually run as many times as neccessary.

03. What are the `SOLID` principles?

    >Single Responsibility, Open Closed, Liskov Substitution, Interface Segregation, Dependency Inversion

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```
    fruit.forEach(item => {
    > if(item == pineapple){
        
    }

    })

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > you.friends.push(them.name)
    them.friends.push(you.name)

06. Give an example of a JavaScript `Conditional`:

    > if(example == 5){
        example = 6
    } else{
        example = 5
    }

07. What is the main difference between `parameters` and `arguments`?

    > Arguments are given in the html code which js functions pull into the parameter section for their code.

08. Instead of writing everything to the console, what is a better way to debug your code?

    > you can check the error logs.

09. What is the difference between a `primitive` value and a `reference` value?

    > Reference value references an element from an object or array, while primitive creates it's own element that is standalone.

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for(i = -100; i > 100; i++){
        console.log(i)
        i++;
    }
