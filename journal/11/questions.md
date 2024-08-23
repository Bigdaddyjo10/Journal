# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | Inheritance in C# allows you to create a new class that is based on an existing class |

1. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | In C#, a class that inherits from another class gets most of its features:
    Yes: It inherits public and protected members (like methods and properties).
    No: It doesn't inherit private members or constructors. |

3. How does ***accessibility*** affect inheritance?

  > | Accessibility in inheritance controls what a derived class can use:
      Public: Inherited and usable everywhere
      Protected: Inherited and usable in the derived class.
      Private: Not usable in the derived class
      Internal: Usable within the same project |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | A PRIMARY KEY uniquely identifies each record in a table. A FOREIGN KEY links one table to another by referencing the PRIMARY KEY of another table, creating a relationship between the two tables |

5. What is an ***alias***?

  > | An alias is a short or temporary name given to a table or column in a SQL query to make it easier to reference |

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
WHERE patient_doctors.doctorId = [doctor_id]; |