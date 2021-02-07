# Angular Scripts & Command with Meaning for References


##### How to install angular material on application  
	ng add @angular/material
	
##### How to install Bootstrap on application
	Steps  
	* npm i bootstrap jquery popper --save  
	* set path in angular.json 
		like "./node_modules/bootstrap/dist/css/bootstrap.min.css"  
		OR  
		just type @import "~bootstrap/dist/css/bootstrap.min.css" inside style.css

#####	Package.json  
			Details  
				1. Scripts  
					* Name of App
					* Version of App
					* Scripts
					* We can also build our own scripts in package.json (Custom Scripts)  
					* Scripts are starting point of your learning if you don't know about app just check package.json and usage of scripts  
					
				2. Dependencies  
					* All the modules/libraries you MUST have to run in production environment
					* The production code will mostly to optimized/minimum
					
				
				
				3. devDependencies  
					* All the modules/libraries to develope to your Application  
					* We may add packages/modules but we may not use them sometimes
					
	# 	Package-lock.json  
			It contains all the details of package.json libraries  
			
##### Angular CLI  
		* Schematics
			ng serve
			ng build
			ng test
			ng lint
			ng e2e
			etc
		
		* Commands
			ng new <Project_Name>
			ng generate component <component_name>
			ng generate module	<module_name>
			ng generate pipe <pipe_name>
			ng directive <directive_name>
			etc
##### Angular Modules  

		1. Angular is a modular-based architecture 
			- There are lot of modules which are built-in 
			- Examples 
				- BrowserModule
				- BrowserAnimationsModule

			- Angular Material Library
				- MatButtonModule
				- MatDropDownModule 

		2. All the code and functionality is grouped in a module 

		3. Whenever you see a @ symbol - it's a decorator 

		4. What modules consist
			- declarations
				- this is where we will add all the components of the module 
			- imports 
				- we can import modules inside a module 
			
			- providers 
				- services that we need will be injected here 
			
			- Bootstrap 
				- what is the first component, the module should load 

			- exports   
				- is to export and expose the component outside of the module  

		5. Every Angular application should have atleast 1 module 

		6. By default, the Angular framework provides us with AppModule 

		7. The AppModule will have a component by the name 
			- AppComponent 
			
		8. Whenever we are building Angular applications 
			- We will always think of Modules first 

			E.g     
				Contacts
				Users 
				Leads
				Opportunites
				Settings 
				Profile 
				Authenctication

			Free User 
				Contacts
				Users 
			Premium User 
				Contacts
				Users 
				Leads
				Opportunites
			Enterprise Users 
				Contacts
				Users 
				Leads
				Opportunites
				Settings 
				Profile 
				Authenctication

		9. Feature Modules 
			- You can turn on or off the modules based on conditions 

		10. Modules - Grouping 
			- components 
			- services 
			- pipes
			- directives 

		11. Create a custom Module 
			ng generate module contacts
			ng generate module leads
			ng generate module settings
			ng generate module Opportunites
			ng generate module authentication 

##### Angular Component Lifecycle Hooks
	###### There are 8 eight lifecycle hooks  	
	
		1. By default we have ngoninit
		
		2. Which ever lifecycle hooks we want to use  
			* import it in the class
			* Extend the implements interface
			* Implement the methods
			
		3. We can have any number of lifecycle hooks implemented