# [bit.ly/ire15sql1](http://bit.ly/ire15sql1)
Cheat Sheet for Session 1

## SQL queries in plain speak (fill in the blanks)
`SELECT` means, "Hey database program, show me stuff in ____ fields."  
`FROM` means, "Hey database program, use ____ table."  
`WHERE` means, "Hey database program, only show me stuff that meets ____ criteria."  
`ORDER BY` means, "Hey database program, sort the stuff by the ____ field, then list it upward or downward."  
`GROUP BY` means, "Hey database program, put certain stuff in one pile, then put different stuff in another pile."  
_Complex queries_ mean, "Hey database program, do a lot of things at once, please."

## Use `SELECT` to initiate a query
It's followed by __field names__, which retrieves data from particular columns (or followed by an asterisk `*`, which retrieves data from all columns).  
Use `FROM` to indicate which __table__ to retrieve data from.

## Use `WHERE` to specify a condition
Use an operator to make a comparison.

|Operator |Comparison measure|
|--------|---------------------|
|`=`     |Equal|
|`<>`    |Not Equal|
|`>`     |Greater Than [After or Later Than]|
|`<`     |Less Than [Before or Earlier Than]|
|`>=`    |Greater Than Or Equal|
|`<=`    |Less Than Or Equal|

Use `AND` to specify a second or third condition.  
Use `OR` to differentiate conditions, i.e. return either/or results.

Use `LIKE` to filter with `%` widcards.  
`ABC%` finds a string that starts with 'ABC'.  
`%XYZ` finds a string that ends with 'XYZ'.  
`%LMNOP%` finds a string that contains 'LMNOP' within it.

## Use `ORDER BY` to filter results downward or upward
Results will return sorted either in ascending or descending order.  
_`ASC` is the default order and is optional to include_  
Use `DESC` to display results Z to A, last to first, most to least, highest to lowest: 9,8,7,6,5,4,3,2,1,0.  
`ASC` displays results A to Z, first to last, least to most, lowest to highest: 0,1,2,3,4,5,6,7,8,9.

#### Remember, the basic query syntax follows this format:

```
SELECT fieldnameA, fieldnameB...
FROM tablenameX
WHERE fieldnameA = datapoint1 AND/OR fieldnameB = datapoint2...
ORDER BY fieldnameA/fieldnameB ASC/DESC;
```
