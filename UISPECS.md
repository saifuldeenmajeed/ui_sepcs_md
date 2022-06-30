# UI SPECIFICATION

This page contains 3 sections:
1. A header (top-aligned, wide as the page is)
2. A database table view (left-aligned)
3. A registration form (right-aligned).

---


## Section 1 (Header) 
This section is a header, wide as the page is (100%), containing 3 elements:

>* Button (left-aligned) to add a new user when clicked after a registration form is filled.
>* CheckBox (left-aligned) to view or hide disabled users.
>* Button (right-aligned) to save the user.

---

## Section 2 (Database Table View)

This section is a table view, the width of half the page (50%), aligned left, and contains 4 columns, where each column contains a filter option. *__Enabled__* column is either true or false, depending on whether the __Enabled__ checkbox is checked or not in the registration form.

_Example_:

| ID  | User Name |         Email         | Enabled  |
|----:|:----------|:----------------------|:---------|
| 1   | AdminUser | adminuser@piworks.net | true     |
| 2   | Test User | testuser@piworks.net  | true     |



---

## Section 3 (Registration Form)

This section is a registration form, width of half the page (50%), aligned right, contains a header titled __New User__, and a body that consists of:

> Text input fields
* __Username__
* __Display Name__
* __Phone__ (Expression Validation check)
* __Email__ (Expression Validation check)

> A dropdown list with _Guest_, _Admin_, _SuperAdmin_ values 

* __User Roles__

> A checkBox

* __Enabled__

`All fields must have a required field validator.`


---

## Events

* __New User__ button shall be clicked if the form is filled correctly.
* __Save User__ button shall save users in the database.
* __Hide Disabled User__ header checkbox shall view or hide users where *__Enabled__* column is *__false__*.
* Assume a user's Enabled status is false if the *__Enabled__* checkbox is not checked.




`Written by Saifuldeen Ali Majeed`.
