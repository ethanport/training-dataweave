# training-dataweave
DataWeave examples for MuleSoft training courses

This is an example Mule project that demonstrates how to apply various formatting to numbers in DataWeave. 

These examples were written for Mule runtime 3.8.3

The dataweave-number-formats folder is a Mule project. You can import this into Anypoint Studio as a Maven project. 

After forking or cloning this repo on your local machine, import a Mavan project into your Anypoint Studio. 
Navigate to the .pom file inside your local copy of dataweave-number-formats. 

The examples demonstrate the use of the {format: ""} syntax to convert a number to a formatted string. In some cases the converted string is again converted back into a number. 

There is a difference between 

`"1234567.89" as :string {format: "#,###.##"}`, 

`"1234567.89" as :string {format: "#,###.0#"}`, and 

`"1234567.89" as :string {format: "#,##0.0#"}`. 

These differences are demonstrated in the various dataweave examples. 

After you load this project into Anypoint Studio, start a debug session. Then open a browser and submit a GET request to `http://localhost:8081`. 

You should see all the results printed out for all the examples. 

To view the number formatting examples, select the DataWeave message processor, then switch between the various flowVars which are set inside the DataWeave message processor. 



