# JavaTask8
# Payment Gateway Simulator

##  Overview
This project is a **Payment Gateway Simulator** built in Java to demonstrate the concepts of:
- **Interfaces**
- **Abstraction**
- **Loose Coupling**
- **Multiple Inheritance using Interfaces**

It simulates different payment methods (Credit Card, Debit Card, UPI, Wallet) and shows how abstraction hides implementation details while keeping the system flexible and extensible.

---

##  Features
- `Payment` interface defines a contract for all payment modes.
- Multiple payment implementations:
  - Credit Card
  - Debit Card
  - UPI
  - Wallet (supports refund and transaction history)
- `PaymentProcessor` class uses **abstraction** to process payments without knowing the actual payment mode.
- Demonstrates **loose coupling** by depending on the `Payment` interface instead of concrete classes.
- Shows **multiple inheritance** in Java using interfaces (`WalletPayment` implements `Payment`, `Refundable`, and `TransactionHistory`).

---

##  Project Structure
PaymentGatewaySimulator.java
├── Payment (interface)
├── Refundable (interface)
├── TransactionHistory (interface)
├── CreditCardPayment (class)
├── DebitCardPayment (class)
├── UpiPayment (class)
├── WalletPayment (class)
├── PaymentProcessor (class)
└── PaymentGatewaySimulator (main class)
