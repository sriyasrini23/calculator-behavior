# Addition

Scenario: Add two numbers
  
  Given I have two numbers to sum

  When I enter "first-number" followed by "+" and "second-number"
  
  Then "sum" is result

Scenario: The numbers are not valid
  
  Given I have a calculator
  
  When I enter invalid input
  
  Then I get an error message

Scenario: Divide by zero error
  
  Given I have a calculator
  
  When I enter second number as zero
  
  Then I get an error message - "Divide by zero error"
