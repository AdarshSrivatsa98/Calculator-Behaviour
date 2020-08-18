# Division

## Scenario: Division by 0 when first operand is any number

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "divide"  
And I type in "Zero"  
And I press "equals"

Then: I see the "Divide by zero error" as the result

## Scenario: Divide 0 by any number

Given:  The calculator is in on state

When: I type in "Zero"  
And I press "divide"  
And I type in "Any number"  
And I press "equals"

Then: I see the "Zero" as the result

## Scenario: Sign rules for operands

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "divide"  
And I type in "opposite signed number"  
And I press "equals"

Then: I see the "Quotient with negative sign" as the result

## Scenario: Division isn't symmetric

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "divide"  
And I type in "Any number except zero"  
And I press "equals"
And I repeat divide(Right,Left)

Then: I see the different result

## Scenario: Division when both operands are 0

Given:  The calculator is in on state

When: I type in "Zero"  
And I press "divide"  
And I type in "Zero"  
And I press "equals"

Then: I see the "zero by zero error" as the result

## Scenario: Recurring decimal case

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "divide"  
And I type in "Recurring decimal number"  
And I press "equals"

Then: I see the "Quotient with certain figures" as the result

## Scenario: More than one "/" as input

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "divide" (More than once)  
And I type in "positive number"  
And I press "equals"

Then: I see the "Quotient with existing operands only once" as the result

## Scenario: Interleaving of different operator

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "divide"(Along with other operator)  
And I type in "positive number"  
And I press "equals"

Then: I see the "Resultant from recent operator" as the result

## Scenario: When operand 2 is not present

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "divide"  
And I press "equals"

Then: I see the "Consider this and gives unity" as the result

## Scenario: Division by any/all operands being fractions

Given:  The calculator is in on state

When: I type in "Fraction number"  
And I press "divide"  
And I type in "Fraction or Any number"  
And I press "equals"

Then: I see the "Quotient with fraction" as the result

## Scenario: Division of more than two numbers  

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "divide"  
And I type in "Any number"  
And I repeat divide operation
And I press "equals"  

Then: I see the "Quotient" as the result
