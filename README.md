# Continues-Development
This is a plan on how to develop software faster and better


# Layers of software

1. Presentation Layer (Front End)
  A. The Presentation / IO Layer Interface
2. IO Layer (Front End)
  A. IO / Function Interface
2. Function Layer ( Front End)
  A. Function / Service Interface
3. Service Layer (Back End)

## Presentation Layer
This layer is seen by the user. It must be designed to look good an peform the functions of getting data into and out of the Application Layer. There should be a clear API between the 
Presentation and the Functional Layer. The Presentation layer may interet return-codes from the Function layer and display them as messages in many different layers. 
Components of the Presentatio layer are:
1. Design, art, fonts, colors. Usability, user research. Looks of the application.

## IO Layer
The IO Layer make the controls shown on the presentation work. It converts user inputs to function inputs and function outputs to 
data displayed to the user. 
1. HTML, CSS, Inputs elements. Output elements.
2. Function Inputs. Takes data from the users, transforms it as neccessar, and puts it into the functions. 
3. Function Outputs. Takes data from functions and transforms it as needed and displayes data to the user

## Function Layer
The Function Layer should perform all the functionality so that the IO layers does not need to do any. 
# Functions
The functions will be "Deep".  This means that one function will do as much work as possible for the caller. The purpose of this is to make the job of connecting the UI to the
functions will be much easer and so that the majority of the testing can be performed on the function and not at the UI stage. 

The kind of work that it will be done within a function are are:

1. Prepratory code. Code that must run before the main task of the function will run.
2. The actual code
3. Post code. Code that must run after the main part of the code is run.
4. Persistant storage. Data that will allow the program run on restart of progrm.  
5. Cache. Storage that can be called on through out the code.
6. Concurance. Code that will return a Return code and then finish processing the command. 

# Return Codes
In order to allow for foreign languages, each function will return a return code. 




