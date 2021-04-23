# Continuous-Delivery
This is a plan on how to develop software faster and better

# Elements of CloudCoin Consinuous Development
1. Three Layers of Software with three development teams.
2. Development on layers happening in parallel to each other. 
3. Serveral Levels/phases being worked on at the same time. 
4. Project Managers find where the bottlenecks are. 
5. Deep Functions (The functions do all the work so UI don't need to)
6. No Branches
7. Daily Integrations. Code is published everyday. With "Feature flags" that point to stable code and code under development. 
8. Allways deployable
9. Tiny Steps
10. Developers can work on future phases when done with current phase
11. Developers can work on other teams/layers when they like if qualified. 
12. Return Codes 
13. Feature Flags
14. Continuous Testing

# Layers of software

1. Presentation Layer (Front End)
 
2. Function Layer ( Front End)

3. Service Layer (Back End)

# Interfaces / Protocols
 1. HTML Naming Conventions (Between the Presentation and IO Layer)
 2. Function Interface (Between the IO and Function Layer) 
 3. Service Protocol (Between the Function and Service Layer) 
 
## Presentation Layer
This layer is seen by the user. It must be designed to look good an peform the functions of getting data into and out of the Application Layer. There should be a clear API between the 
Presentation and the Functional Layer. The Presentation layer may interet return-codes from the Function layer and display them as messages in many different layers. 
Components of the Presentatio layer are:
1. Design, art, fonts, colors. Usability, user research. Looks of the application.
2. HTML, CSS, Inputs elements. Output elements.
3. Function Inputs. Takes data from the users, transforms it as neccessar, and puts it into the functions. 
4. Function Outputs. Takes data from functions and transforms it as needed and displayes data to the user

## Function Layer
The functions will be "Deep".  This means that one function will do as much work as possible for the caller. The purpose of this is to make the job of connecting the UI to the
functions will be much easer and so that the majority of the testing can be performed on the function and not at the UI stage. 

The kind of work that it will be done within a function are are:

1. Prepratory code. Code that must run before the main task of the function will run.
2. The actual code
3. Post code. Code that must run after the main part of the code is run.
4. Persistant storage. Data that will allow the program run on restart of progrm.  
5. Cache. Storage that can be called on through out the code.
6. Concurance. Code that will return a Return code and then finish processing the command. 

Work that needs to be done: 
1. Function Design
2. Return Code Design
3. Function Development
4. Function Testing

# Return Codes
In order to allow for foreign languages, each function will return a return code. 



# Example of Workflow, Skills needed and persons to do that job
## Service Layer Workflow for the 
Task | Skills Needed | Person
---|----|---
Service Design | Network Protocols   | Sean
Service Design Review | Knowledge of Network Protcols | Partha, Alexander
Service Implementation | Needs to know PHP or C | Sergiy, 
Service Implementation Review | Needs to know PHP or C | Sergiy,
Service Testing | Testing Skills | Chernyshov
Deploymnet | RAIDA Administration | Fel
Manager | Managment Skills | Sean

## Function Layer Workflow
Task | Skills Needed | Person
---|----|---
Function Design | Javascript Programming | Alexander, Sean, Partha, 
Function Design Reveiew | Interface Skills | Ravie, Partha, Sergiy
Function Implementation |  Javascript Programming | Alexander, Ravi, Partha
Function Code Review | Javascript Programming | Alexander, Ravi, Partha
Function Testing | Testing | Sergiy, 

## IO Layer Workflow
Task | Skills Needed | Person
---|----|---
Presentation Design | UI / UX |  
Presentation Design Reveiew | Interface Skills | Ravie, Partha, Sergiy
Presentation Implementation |  Javascript Programming | Alexander, Ravi, Partha
Presentation Code Review | Javascript Programming | Alexander, Ravi, Partha
Presentation Testing | Testing | Avisek





