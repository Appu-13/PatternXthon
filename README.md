# PatternXthon


Online Food Ordering System
A simple Object-Oriented Design (OOD) project modeled using a UML class
diagram in StarUML. The system demonstrates five design patterns and
includes an additional MVC package.

Design Patterns Used

## Design Patterns Used

| Design Pattern | Classes in the UML | Purpose |
| :--- | :--- | :--- |
| **Factory** | `Food`, `FoodFactory`, `Pizza`, `Burger`, `Sandwich` | Creates different food objects through a common factory. |
| **Singleton** | `DatabaseConnection` | Provides access to a shared database-connection instance. |
| **Observer** | `Order`, `Observer`, `CustomerObserver` | Notifies registered observers when an order status changes. |
| **Strategy** | `Payment`, `PaymentStrategy`, `UpiPayment`, `CardPayment`, `CashOnDelivery` | Supports interchangeable payment methods. |
| **Decorator** | `Food`, `FoodDecorator`, `ExtraCheese`, `ExtraToppings` | Adds optional food customizations and their additional cost dynamically. |



Additional Architecture
The UML project also contains an MVC (Model--View--Controller)
package:
- FoodModel -- manages food and order data.
- FoodView -- displays menu, cart, order details, and payment
  status.
- FoodController -- coordinates user actions between the model and
  view.
  
Main System Components
The Core Domain package contains the main entities:

- Customer -- represents a user of the food-ordering system.
- Restaurant -- represents a restaurant that displays a menu and
  handles orders.
- Cart and CartItem -- maintain selected food items, quantities,
  and totals.
- Delivery -- manages delivery assignment and delivery status.

Typical Workflow

1. A customer browses the restaurant menu.
2. FoodFactory creates the selected food object.
3. Decorators such as ExtraCheese or ExtraToppings can customize
   the food.
4. The selected items are added to the cart.
5. An order is created and managed.
6. The customer selects a payment method through the payment strategy.
7. When the order status changes, registered observers receive updates.
8. The restaurant processes the order and delivery information is
   updated.
   
Project File

- OnlineFoodOrderingSystem.mdj -- editable StarUML project
  containing the UML model and class diagram.
- OnlineFoodOrderingSystem_UML_Explanation.docx -- detailed
  explanation of the classes, attributes, operations, design patterns,
  relationships, workflow, and viva questions.
  
How to Open

1. Install and open StarUML.
2. Select File → Open.
3. Choose OnlineFoodOrderingSystem.mdj.
4. Open the class diagram from the Model Explorer.

Notes

- This is an academic OOD/UML modeling project. The .mdj file
  represents the design; it is not a running food-ordering
  application.
- In the supplied UML, the Singleton class is named
  DatabaseConnection. Its instance attribute and getInstance()
  operation are shown, but a private constructor is not explicitly
  represented.
- The project includes the five requested design patterns and an
  additional MVC package.
  
Author

Name: Yathin S,
USN: 1MP24CG063,
Class/Section: 5th Semester, CSD
