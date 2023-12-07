# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | Makes it so you can use the same data over and over without rewriting it. |

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | Very similar to SQL where it makes it so if you inherit something then you do not have to continue to write it over and over. |

3. How does ***accessibility*** affect inheritance?

  > | Depends on wether they are visible or not. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | Primary key can only happen once per table, while a foreign key can happen multiple times as long as it matches the reference. |

5. What is an ***alias***?

  > | Gives a column in a table a temporary name |

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > | SELECT patients.*
FROM patients
JOIN patient_doctors ON patients.id = patient_doctors.patientId
WHERE patient_doctors.doctorId = @doctorId; |
