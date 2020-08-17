# Multiplication

Scenario: Multiply two numbers
  
  Given I have two numbers to multiply

  When I enter "first-number" followed by "x" and "second-number"
  
  Then "product" is result

Scenario: The numbers are not valid
  
  Given I have a calculator
  
  When I enter one or more inputs that are invalid or not numbers
  
  Then I get an error message - "Invalid input"
