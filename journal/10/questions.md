# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > | How the module system works with .Net or the C# convection. It is similar to export that we used before. |

02. What is the difference between a `class` and an `interface`?

  > | Class has a definition and implementation while interface only has a definition.  |

03. What is the method that returns an instance of a class, yet it has no return type?

  > | Void |

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

  > | Public |

06. In the Car example what is `string` an indication of?

  > | the return time |

07. In the Car example what is `abstract` preventing?

  > | Preventing the car from being instantiated. |

08. In a SQL table, what is the difference between information in a row and information in a column?

  > | Each row represents a unique record, and each column represents a field in the record. |

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > | CREATE TABLE
    IF NOT EXISTS ingredients(
        id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
        createdAt DATETIME DEFAULT CURRENT_TIMESTAMP COMMENT 'Time Created',
        updatedAt DATETIME DEFAULT CURRENT_TIMESTAMP ON UPDATE CURRENT_TIMESTAMP COMMENT 'Last Update',
        name VARCHAR(54) NOT NULL,
        quantity VARCHAR(1000) NOT NULL,
        recipeId INT NOT NULL,
        creatorId VARCHAR(255) NOT NULL,
        FOREIGN KEY(recipeId) REFERENCES recipes(id) ON DELETE CASCADE,
        FOREIGN KEY(creatorId) REFERENCES accounts(id) ON DELETE CASCADE
    ) default charset utf8 COMMENT ''; |

10. In SQL how can you query more than a single table? Provide an example.

  > | JOIN whatever you want ON |
