# Demo
Feature: Form_filling

Scenario: Not Filling mandatory fields
	Given The user is on the website
	And user has not filled the data in mandatory "<field>"
	When the user chooses to proceed further
	Then user must be notified with a "<message>" as mandatory field
	And must stay on the page
	
Scenario: Filling mandatory fields
	Given The user is on the website
	And user has filled the data in mandatory "<field>"
	When user chooses to proceed further
	Then user will be navigated forward
	
