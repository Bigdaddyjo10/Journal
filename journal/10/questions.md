# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | namespace is used to organize code and prevent naming conflicts by grouping related classes, structs, and other types together. |

02. What is the difference between a `class` and an `interface`?

  > | Class: Defines a blueprint for creating objects, including data and methods. Interface: Defines a contract that classes can implement, specifying methods but not their implementation. |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | constructor |

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > | public |

06. In the Car example what is `string` an indication of?

  > |  string indicates that the Start() method will return a value of type string. |

07. In the Car example what is `abstract` preventing?

  > | abstract is preventing the Car class from being instantiated directly. You cannot create an object of the Car class; instead, you must create objects of classes that inherit from Car and implement its abstract members |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | Row: A single record in the table. Column: A specific type of data in the table. |

1.  Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE characters (
    id INT,
    name VARCHAR(255),
    age VARCHAR(255),
    description VARCHAR(255)
);
|

10. In SQL how can you query more than a single table? Provide an example.

  > | To query more than one table in SQL, you can use a JOIN |
