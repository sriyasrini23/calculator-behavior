# Addition

Scenario: Add two numbers
  
  Given I have two numbers to sum

  When I enter "first-number" followed by "+" and "second-number"
  
  Then "sum" is result

Scenario: The numbers are not valid
  
  Given I have a calculator
  
  When I enter one or more inputs that are invalid or not numbers
  
  Then I get an error message - "Invalid input"
