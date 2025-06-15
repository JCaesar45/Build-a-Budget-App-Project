````markdown
# 💰 Budget App

A simple Python-based command-line application to track budget categories (like Food, Clothing, etc.) using object-oriented programming. It allows users to deposit, withdraw, transfer funds, and visualize category-wise spending with a vertical bar chart.

---

## 📦 Features

- Object-Oriented `Category` class
- Transaction ledger for deposits and withdrawals
- Balance calculation
- Fund transfers between categories
- Accurate check for sufficient funds
- Text-based spend chart showing percentage distribution

---

## 🧠 Class Overview

### `Category`

```python
Category(name)
```

Creates a new budget category with a given name and initializes an empty ledger.

#### 🔹 Methods

```python
deposit(amount, description="")
```

Adds a deposit to the ledger.

```python
withdraw(amount, description="")
```

Subtracts a withdrawal from the ledger if funds are available.

```python
get_balance()
```

Returns the current balance of the category.

```python
transfer(amount, other_category)
```

Transfers funds between two categories.

```python
check_funds(amount)
```

Returns `True` if there are sufficient funds, `False` otherwise.

```python
__str__()
```

Formatted string of the ledger showing all transactions and total.

---

## 📊 Spend Chart

### `create_spend_chart(categories)`

Generates a bar chart showing percentage of total spending per category.

```python
print(create_spend_chart([food, clothing, entertainment]))
```

Sample Output:

```
Percentage spent by category
100|          
 90|          
 80|          
 70|          
 60| o        
 50| o        
 40| o        
 30| o        
 20| o  o     
 10| o  o  o  
  0| o  o  o  
    ----------
     F  C  E  
     o  l  n  
     o  o  t  
     d  t  e  
        h  r  
        i  t  
        n  a  
        g  i  
           n  
           m  
           e  
           n  
           t  
```

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/budget-app.git
   cd budget-app
   ```

2. Run the main script in your terminal:

   ```bash
   python budget.py
   ```

3. Explore with your own categories and transactions.

---

## 🧪 Testing

Use your favorite Python testing framework (e.g., `unittest`) to validate each method. Integration with FreeCodeCamp’s test suite is also supported for learners.

---

## 🛠️ Tech Stack

* Python 3.x
* Object-Oriented Programming
* CLI interface

---

## ✍️ Author

**Jordan Leturgez**
Fort Wayne, Indiana, USA
*Virtual Assistant | Data Analyst | Developer | Educator*

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

```
