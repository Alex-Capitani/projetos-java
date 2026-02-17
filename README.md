# 📦 Java Encapsulation Example – Access Modifiers

## 📌 Overview
This project demonstrates the concept of **encapsulation in Java**, focusing on **communication restrictions between objects** using **access modifiers**.

The activity aims to show how attributes and methods can have different visibility levels and how this affects access and data protection in object-oriented programming.

This example was developed as part of Java OOP studies.

---

## 🎯 Objective
The goal is to understand:

- Object communication
- Encapsulation principles
- Use of access modifiers (`public`, `private`)
- Difference between local variables and class attributes
- Controlled access to internal data

---

## 🧱 Project Structure
Example structure:

src/
└── model/
└── Pai.java


---

## 🧠 Concepts Applied

### Encapsulation
Encapsulation protects object data by restricting direct access and allowing manipulation only through methods.

### Access Modifiers Used
| Modifier | Visibility |
|-----------|------------|
| `public`  | Accessible from any class |
| `private` | Accessible only inside the class |

---

## 📄 Class Description

### Class: `Pai`
Represents a father entity with personal and salary information.

#### Attributes
``java
public String nome;
public int idade;
private double salario;

- nome and idade are public.
- salario is private to protect sensitive data.

## Methods

**cadPai(...)**
Registers father data.

public void cadPai(String nm, int anos, int sal)

⚠ Note: nome inside the method is declared as a local variable, not updating the class attribute. The correct assignment would be:

this.nome = nm;

**calcSalario()**
Private method that increases salary by 10%.

private void calcSalario()

Only accessible internally.

---

**impPai()**
Displays father information.

public void impPai()

---

## How to Run

Open project in NetBeans or IntelliJ.

Compile the project.

Execute a main/test class calling the methods.

Example usage:

Pai pai = new Pai();
pai.cadPai("Carlos", 50, 5000);
pai.impPai();

## Technologies Used

- Java SE
- Object-Oriented Programming
- Encapsulation
- Access Modifiers

## Learning Outcome

- This project reinforces:
- Data protection using encapsulation
- Proper visibility control
- Class organization practices

## Author

Alex Capitani
Java backend developer
