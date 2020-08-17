# Subtraction

Scenario: Subtract two numbers
  
  Given I have two numbers to subtract

  When I enter "first-number" followed by "-" and "second-number"
  
  Then "difference" with sign is result

Scenario: The numbers are not valid
  
  Given I have a calculator
  
  When I enter one or more inputs that are invalid or not numbers
  
  Then I get an error message - "Invalid input"
