The application represents functionality for the creation and management of water vending machines.

# Water Vending Machine — Lab 2

## Class Overview
The project is based on the **Water Vending Machine** class from Lab-1, updated to follow **encapsulation and properties** principles.

---

## Encapsulation
All class fields are **private**.  
External access is provided **only through public properties**.

### Private Fields
- `_cashAmount : decimal`
- `_cashCapacity : decimal`
- `waterCapacityLiters : int`
- `waterLeftLiters : int`
- `refillDate : DateTime`
- `state : MachineState`
- `operatorName : string`
- `phone : string`
- `companyName : string`

---

## Properties
- `WaterCapacityLiters`
- `WaterLeftLiters`
- `RefillDate`
- `State`
- `OperatorName`
- `Phone`
- `CompanyName`
- `Address` — **auto-property with default value**
- `WaterSoldLiters` — **computed property**  
  (`WaterCapacityLiters - WaterLeftLiters`)

At least one property uses **different access levels** for `get` and `set`.

---

## Methods
- `PutMoney(decimal cash)`
- `TakeWater(int volume)`
- `Refill()`
- `WithdrawCash()`

Public methods internally use **private helper methods** to hide implementation details.

---

## Program Logic
- All field access in `Program.cs` is done **via properties only**
- Input values are validated before assignment

---

## Menu
1. Add object  
2. View all objects  
3. Find object  
4. Demonstrate behavior  
5. Delete object  
0. Exit  
