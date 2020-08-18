# Multiplication

## Scenario: Result overflow

Given:  The calculator is in on state

When: I type in "Big number"  
And I press "multiply"  
And I type in "Big number"  
And I press "equals"

Then: I see the "Stack Overflow" as the result

## Scenario: Signs of the numbers

Given:  The calculator is in on state

When: I type in "A number"  
And I press "multiply"  
And I type in "A number with opposite sign"  
And I press "equals"

Then: I see the "Solution with negative sign" as the result

## Scenario: Zero value multiplication

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "multiply"  
And I type in "Zero"  
And I press "equals"

Then: I see the "Zero" as the result

## Scenario: Multiplication by 1

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "multiply"  
And I type in "Unity"  
And I press "equals"

Then: I see the "same number" as the result

## Scenario: Decimal value multiplication

Given:  The calculator is in on state

When: I type in "Number with decimal values"  
And I press "multiply"  
And I type in "Number with decimal values"  
And I press "equals"

Then: I see the "Solution with decimal values" as the result

## Scenario: Irrational value multiplication

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "multiply"  
And I type in "Irrational number"  
And I press "equals"

Then: I see the "Irrational solution with limited figures" as the result

## Scenario: Simple multiplication

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "multiply"  
And I type in "Any number"  
And I press "equals"

Then: I see the "Solution" as the result

## Scenario: Rational multiplication

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "multiply"  
And I type in "Any number"  
And I press "equals"

Then: I see the "Solution" as the result

## Scenario: Decimal & integer multiplication

Given:  The calculator is in on state

When: I type in "Decimal or Integer number"  
And I press "multiply"  
And I type in "Any number"  
And I press "equals"

Then: I see the "Solution with decimal values" as the result

## Scenario: More than two numbers multiplication

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "multiply"  
And I type in "Any number"  
And I repeat multiplication operation  
And I press "equals"  

Then: I see the "Solution" as the result

## Scenario: Complex number multiplication

Given:  The calculator is in on state

When: I type in "Complex number"  
And I press "multiply"  
And I type in "Complex number"  
And I press "equals"

Then: I see the "Solution along with complex parts" as the result

## Scenario: Range of operand exceeds allowed limit

Given:  The calculator is in on state

When: I type in "Any number exceeding limit"  
And I press "multiply"  
And I type in "Any number exceeding limit"  
And I press "equals"

Then: I see the "Solution with arrested input figures" as the result

## Scenario: Pressing "multiply button" more than once

Given:  The calculator is in on state

When: I type in "positive number"  
And I press "multiply" (More than once)  
And I type in "positive number"  
And I press "equals"

Then: I see the "Solution performing operation once" as the result

## Scenario: Interleaving operators (Press *, then press /, then press +)

Given:  The calculator is in on state

When: I type in "Any number"  
And I press "multiply"(Followed by other operator)  
And I type in "positive number"  
And I press "equals"

Then: I see the "Solution of recent operator" as the result

## Scenario: Decimal value capping

Given:  The calculator is in on state

When: I type in "Decimal value exceeding limit"  
And I press "multiply"  
And I type in "Decimal value exceeding limit"  
And I press "equals"

Then: I see the "Solution with arrested input decimal figures" as the result
