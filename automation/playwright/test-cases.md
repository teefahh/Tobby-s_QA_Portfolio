# Test Cases For Demo QA Login functionality

ID |      Scenario               | Steps     | Expected Results | Actual Results   | Status  
----------------------------------------------------------------------------------------------    
Tc 01 | Login with Valid username & Password| Input valid username & Password | User should be logged in successfully | successfully | Pass
Tc 02| Login with invalid username and password| Input invalid username & Password| Access should be denied, error message: invalid credentials should be displayed| Access is denined, appropriate error message is displayed| pass
Tc 03| Blank username & Password| Leave username & Password field blank| Access denined, Prompt user for valid credentials| Pass