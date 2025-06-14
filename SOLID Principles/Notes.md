# SOLID Principle

So before jumping into a SOLID principle first lets understand why it was developed

In real world when we write code there are various issues in our code  
the issues can be:  
- Tightly Coupled  
- Poor Scalability  
- Difficult to understand the code  
- Bug prone changes and much more

So to overcome this issue SOLID Principles came into picture.  
Solid principles was Developed by **C Martin** also known as **Uncle BOB**.  
After understanding and implementing this principles in our day to day programming life we will be able to deliver a very good quality of code.

**S** stands for **Single Responsibility**  
**O** stands for **Open/Closed**  
**L** stands for **Liskov Substitution**  
**I** stands for **Interface Segregation**  
**D** stands for **Dependency Inversion**

Let's try to understand this one by one with an example.

---

## Single Responsibility

Let's suppose i have a real world city and i need to implement the bus system in that city, so to develop that i need to have **Bus** and **Driver** so that Driver can drive a bus.  
But if i tell driver to collect the tickets, maintain the bus, drive the bus, so for driver it will be over burden with the responsibilities. 

So similarly while coding when we create any class then that class should not be overburden with the responsibility.  
Example: we created one class and in that same class we are having all features/responsibilities like:
- login
- registration
- OTP
- email sending
- reminder
- reports etc.

By doing this we are overburdening the class with multiple responsibilities.  
So to solve this we need to follow **Single Responsibility Principle** where driver job is just to drive, where one class will handle only one responsibility.

---

## Open/Closed

Now suppose there are few routes/road in your city and your city grows tomorrow now you want to extend this routes/roads.  
You will not just go and demolish the old route/roads and redevelop that all again just because you need to extend your routes/road.  
Instead of touching the existing route you can have a new route, you can add new routes/roads to your bus system.

Similarly the second principle is **Open/Closed principle** where it says:
- It should be open for extension (your class, methods) but closed for modification.

You should not write the code in such a way that every time you go and touch the main code, you should be only extending that code or write something top on it.

---

## Liskov Substitution

Now moving to next principle we have **Liskov Substitution**.  
If tomorrow new electric busses will come then driver should be able to drive that bus also, it should not in a way that old driver should not be incompetent.

Similarly you should not design new function out of the box where old functionality is not in used.  
We should design in such a way that old bus / parent is also used. It should not go unused.  
Even if you design the electric bus the driving should be same then driver should not be incompetent.

---

## Interface Segregation

Next principle is **Interface Segregation** where:

- In simple words don't give bus driver too many options/control on his driving panel which will create unnecessary confusion for a driver to understand that controls.  
- Similarly we should not create unnecessary interfaces and classes where people are confused to use and see which class or interface to use, what it's going to do for me, how this is going to help me.

---

## Dependency Inversion

Lastly **Dependency Inversion** is nothing but:

- A bus should be able to charge or refill her tank at any pump/station.

---
