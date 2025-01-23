# Unexpected Null Handling in Addition Function

This repository demonstrates a potential bug in JavaScript related to null value handling during addition.  The `foo` function is designed to add two numbers, but its treatment of null values might not align with all expectations.  The bug and its solution are detailed in separate JavaScript files.

## Bug Description

The `foo` function correctly handles null inputs by returning 0.  However,  a more robust solution might be needed if the function needs to handle other types of non-numeric input.  Currently, the function only handles explicit null values and will cause an error if other non-numeric values are supplied.

## Solution

The solution improves the handling of non-numeric inputs by performing type checking. It uses typeof to check if the inputs are numbers. If not, it returns an error message, making the behavior more predictable and less error-prone. 