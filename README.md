How to use streamlit tutorial

[1] Installing packages and generating a virtual environment
Create the folder
Open the terminal under that folder
pip install virtualenv
-	It is important to install a virtual environment 
o	Clean set up and won’t be affected by other library packages installed for other projects
o	To avoid conflicts between other packages as some projects may use different versions of the same library
o	If the project you have is on a beginner level where you have many dependencies to install, it can slow down your machine when you do process them all at the same time
-	This command only needs to be done once – at the beginning of the project
-	To call this virtual environment – activate using env\scripts\activate
o	If it doesn’t work due to security issues, you need to change the execution policy to allow scripts to run
Go to Powershell and input the code: 
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
Ensure same directory when using the command prompt to install virtualenv

[2] Introduction of Streamlit
-	What is streamlit (Adrien Treuille created it in 2018)
o	Streamlit is a Python library that makes it easy to create interactive web applications for data science and machine learning projects.
o	The Python backend of our app represents the server while the frontend that is viewed through a browser like chrome or safari is the client, and if the app is developed locally like what we’re doing now, your computer runs both the server and the client
-	Why is it important
o	It allows you to create interactive web applications with only python
o	Before Streamlit: You would need to know web development HTML, Java Script and a backend framework like Django or Flask to even build a web application and keep testing it until you could deploy your app properly
o	Plus, you could develop the barebones structure of your code and test it right away
[3] Run the application
-	Step 1: import streamlit and create a title
-	Step 2: run the app in the terminal, please type streamlit run app.py
[Break] Work on individual issues by students 🙏😅
 

[4] Proceed with Streamlit
-	Here’s the dataframe of weather and sales data where
o	The weather data is the line chart and the monthly sales data is the bar chart
-	Refresh the webpage or deploy your app 
-	Sidebar application: 
o	Here’s the data on Tina, me, Ibraheem, Rex about their favourite colour and where they are from
-	Layout and containers
o	Using the simple chart from before you can split the charts into 3 columns
o	Refresh the webpage to display the change
-	Callback functionality
o	Using buttons can be very helpful in calling an action, especially in submitting forms or collecting user input, the callback functions can process these inputs and provide feedback or results
o	In this example, clicking the button titled: What is streamlit gives you the text written within st.write
[5] Deployment
-	First go to Github and create an account and a new repository
-	Leave it public and name it StreamlitWorkshop
-	From there, create a new file that will hold our python code
-	Upload the code from the archive section which is essentially the same thing as what we had before
-	Create an account on streamlit, log in with your Github account so you can link your repositories later
-	You can select from the main branch of your repository and the main file path will follow

[6] Going Further
-	We have a function that analyzes the text, we have the text input here, and we will render an image using DALL-E-3 
-	An image function and text function are generated separately using different OPENAI language models
-	Now to set it up on Github by overwriting the existing code in app.py with the new code
-	Go to the Requirements.txt file and add openai
-	Go into Secrets, and copy the OPEN_API_KEY from the app.py code and paste the API key
