# rs_calisma
# RoofStacks
## _Case Study_



[![N|Solid](https://github.com/Eyyupguzel/roofstacks/blob/main/roof_stacks/src/test/java/Karate_Features/roof.png)](https://nodesource.com/products/nsolid)




# Intro




There are scenarios of service automations. An explanation of these scenarios and a general comment about the project have been added.Karate framework was used to write automation.While writing the cases, the name of the scenario and the description of the scenario, the risk of scenario, the precedence of the scenario, regression type, expected result,status were determined.



[![N|Solid](https://github.com/Eyyupguzel/roofstacks/blob/main/roof_stacks/src/test/java/Karate_Features/karate.png)](https://nodesource.com/products/nsolid)



> Post method is used for Crate User service.Response time control was made to be less than 6 seconds.Checked that the userId value is not null as a result in the post methods.Controls were made considering the minimum and maximum values.Required fields were also checked.Since some cases are similar, they were written by changing the values in the same scenario with the scenario outline property.Even if we write an incorrect case because the services were mocked, status 200 was returned, so their status was determined as 200 while writing the scripts.Correct status values added as comments.



# Auth - Token Scenarios
| Scenario Name | Scenario Description | Steps | Risk | Precedence | Regression Type | Expected Result | Status |
|-------------| ------ | ------| ------ | ------| ------ | ------ | ------ |
| Fetch Token Informations - Success Fetch Token Information | This request fetches the id token and another authentication info with a registered email and correct password. | **_Given_** request data create with " email " and " password ". **_When_** a POST request is send to "https://europe-west3-test-goart.cloudfunctions.net/api/auth/token". **_Then_** the status code is 200. | High | High | Daily | Status Code 200 | OK |

## _Karate Reports_
