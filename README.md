# 🏨 Hotel Management System

A console-based hotel management application built with Java for managing bookings, food orders, and billing. Features automatic data persistence using Java Serialization.

## ✨ Features

- **Room Booking & Availability**: Manage Luxury/Deluxe and Single/Double room types with real-time availability tracking
- **Food Service**: Order food directly to rooms with automatic cost integration
- **Billing System**: Generates detailed invoices at checkout with itemized charges
- **Auto-Save Persistence**: Automatic data backup to local file on exit and reload on launch

## 🚀 Quick Start

### Prerequisites
- Java Development Kit (JDK) 8 or higher

### Compilation
```bash
javac Main.java
```

### Execution
```bash
java Main
```

## 💰 Room Rates (Per Day)

| Room Type | Price | Amenities |
|-----------|-------|-----------|
| Luxury Double | Rs. 4,000 | AC, Breakfast |
| Deluxe Double | Rs. 3,000 | Breakfast |
| Luxury Single | Rs. 2,200 | AC, Breakfast |
| Deluxe Single | Rs. 1,200 | Breakfast |

## 🛠️ Technical Concepts

### Object-Oriented Programming
- **Inheritance**: `Doubleroom` class extends `Singleroom` for code reusability
- **Encapsulation**: Room and booking data protected within classes
- **Polymorphism**: Flexible room type handling

### Data Persistence
- **Serialization**: Java `Serializable` interface for object-to-file storage
- **File I/O**: Automated backup file generation

### Concurrency
- **Multithreading**: Background thread handles file writing operations without blocking main application

## 📁 File Structure

```
.
├── Main.java           # Entry point and main application logic
├── Singleroom.java     # Single room class definition
├── Doubleroom.java     # Double room class (extends Singleroom)
└── backup              # Auto-generated data persistence file
```

## ⚠️ Important Notes

- **Do not delete the `backup` file** - it contains all your saved hotel data
- Data is automatically saved on application exit
- Previous session data is restored on application launch

## 📝 License

This project is open source and available for educational purposes.

---

**Made with ☕ and Java**
