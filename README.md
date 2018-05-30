
# api-test
Feature: CHECK API STATUS

  Scenario: GET request
    
    When I perform the following step:
    I send a GET request to "/api/books" 
    Then the response status should be "200"
    
    
  Scenario: POST request with params
    
    When I perform the following step with table:
    I send a POST request to "/api/books" with the following:
     | title     | Metaprograming ruby |
     | publisher | Pragprog            |
    Then the response status should be "201"
    
    

INSTRUCTION
   1. Create a working API automation testing framework using a programming language of your choice
   2. Create new branch and Push your code back to github
    
