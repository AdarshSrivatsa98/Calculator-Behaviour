# Addition

## Scenario: Addition of two positive numbers

Given:  The calculator is turned on

When: I type in "positive number"
And I press "plus"
And I type in "positive number"
And I press "equals"

Then: I see the "added number" as the result

## Scenario: Addition of two negative numbers

Given:  The calculator is turned on

When: I type in "negative number"
And I press "plus"
And I type in "negative number"
And I press "equals"

Then: I see the "added number with negative sign" as the result

## Scenario: Addition of fractions

Given:  The calculator is turned on

When: I type in "Integer or Fraction number"
And I press "plus"
And I type in "AtleastOne(Fraction) or Integer number"
And I press "equals"

Then: I see the "Fraction or Integer resulted from addition" as the result

## Scenario: Addition of +ve and -ve number

Given:  The calculator is turned on

When: I type in "positive/negative number"
And I press "plus"
And I type in "negative/positive number"
And I press "equals"

Then: I see the "difference of numbers with sign of resultant number" as the result

## Scenario: Addition of decimals

Given:  The calculator is turned on

When: I type in "Integer/Decimal number"
And I press "plus"
And I type in "AtleastOne(Decimal) or Integer number"
And I press "equals"

Then: I see the "Decimal or Integer resulted from addition" as the result

## Scenario: Typing operator more than once

Given:  The calculator is turned on

When: I type in "Any number"
And I press " plus (More than once)"
And I type in "Any number"
And I press "equals"

Then: I see the "Syntax Error" as the result

## Scenario: Addition of more than 2 numbers

Given:  The calculator is turned on

When: I type in "Any number"
And I press "plus" between operands
And I type "Any number"
And I press "equals"

Then: I see the "added number" as the result

## Scenario: Adding numbers where the result goes out of range

Given:  The calculator is turned on

When: I type in "Any number"
And I press "plus"
And I type "Any number" 
And I press "equals"

Then: I see the c"Reached Maximum limit" as the result

## Scenario: 6+* is provided as input?

Given:  The calculator is turned on

When: I type in "Any number"
And I press "plus" along with invalid input
And I type "Any number" 
And I press "equals"

Then: I see the "Syntax Error" as the result

## Scenario: Identify operation

Given:  The calculator is turned on

When: I type in "Any number"
And I press "plus"
And I type "Zero" 
And I press "equals"

Then: I see the "return same number" as the result

## Scenario: Converse operation

Given:  The calculator is turned on

When: I type in "Any number"
And I press "plus"
And I type "Any number" 
And I press "equals"
And I repeat plus(Right,Left)

Then: I see the same result
