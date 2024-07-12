# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > | const, let |

02. What is the definition of a function?

    > | A function runs a specific block of code that runs when it is called.|

03. What are the `SOLID` principles?

    > | S — Single responsibility, O — Open closed, L — Liskov substitution, I — Interface segregation, D — Dependency Inversion  |

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > | fruit.splice(2)|

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

    > | you.friends.push(them) them.friends.push(you) |

06. Give an example of a JavaScript `Conditional`:

    > | : ? |

07. What is the main difference between `parameters` and `arguments`?

    > | A parameter is a variable in a function definition. It is a placeholder and hence does not have a concrete value. An argument is a value passed during function invocation |

08. Instead of writing everything to the console, what is a better way to debug your code?

    > | console.log() |

09. What is the difference between a `primitive` value and a `reference` value?

    > | a primitive variable's information is stored as the value of that variable, whereas a reference variable holds a reference to information related to that variable |

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > | for (let i = -100; i <= 100; i++) |
