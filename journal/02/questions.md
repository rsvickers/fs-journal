# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | var, let. const |

02. What is the definition of a function?

    > | a function does a specific task when they are invoked. |

03. What are the `SOLID` principles?

    > | It is an acronym to improve the quality of the software.
    stands for S = single responsibility principle
    O = open-closed principle
    L = Liskov substitution principle
    I = Interface segregation principle
    D = Dependency inversion principle |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | delete fruit[2] |

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

 | you.friends.push(them)
    them.friends.push(you) |

06. Give an example of a JavaScript `Conditional`:

    > | if statements  |

07. What is the main difference between `parameters` and `arguments`?

    > | parameters are the made up words while the arguments are the actual values. |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | set break points or comment out certain code |

09. What is the difference between a `primitive` value and a `reference` value?

    > | primitive values are only stored in a variable. while reference values are stored in the memory and can constantly be referenced.  |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for (let i = -100; i <= 100; i++) {
    console.log(i)
} |
