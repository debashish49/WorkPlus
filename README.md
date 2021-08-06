# WorkPlus
_**Won 1st Place at the Japan Inter-School Hackathon 2021**_

WorkPlus is a collaborative platform designed for workplace communication that simultaneously promotes a healthy and fruitful lifestyle for all the employees. Not only does it allow you to share tasks and files with your teammates and communicate with them through an interactive chat window, WorkPlus also enables you to track your personal and team fitness levels and engage in fun, rewarding fitness and trivia challenges, making “work from home” a more enjoyable & productive experience!

## Project Objective
Due to Covid-19, remote working has skyrocketed, especially in the IT industry, leading to an increase in work hours. As a result, fitness, mental health and productivity have taken a massive toll, so our project will aim to solve these underlying issues by building an application that promotes a healthy mode of living in the current working environment.

## Video Demo
[WorkPlus: Official Hackathon Demo (YouTube)](https://youtu.be/RHhPdILZCoQ)

[![name](https://user-images.githubusercontent.com/69211573/128547266-6ea800a8-90dc-4392-a47b-8e7d0ae23df4.png)](https://youtu.be/RHhPdILZCoQ)

## Project Features

### Fitness & Team Bonding Features

- **Connect your Fitbit Account**: WorkPlus allows you to authorize your Fitbit account with your profile, and displays relevant health and fitness data to you and your teammates! 

- **Upload your daily Nike Run**: WorkPlus offers a daily 2km running challenge where you can upload a screenshot of your run today using the Nike Run Club App, and our program rewards you with points after proofreading the upload using Python's AI and Image Recognition!

- **Trivia of the Day**: WorkPlus assigns you a daily trivia question that rewards you with points when answered correctly!

- **Incentive Point System**: WorkPlus has an in-built point system that is used as an incentive to keep workers healthy. Completing tasks like the Nike Run Club daily 2km challenge & the Trivia of the Day reward you with points that get added up to your tally for the month. The point system restarts each month. WorkPlus displays you your current point tally and also the team's cumulative tally. Users do not get to view their peers' points in order to avoid unhealthy competition. The team leader, however, can see everybody's points. At the end of every month, the person with the most points can be rewarded for his efforts, and the company/team has the full freedom to come up with a prize. For instance, one of the best suggestions on behalf of WorkPlus is for the team to donate $1 or ¥100 per point achieved by the team as a whole to a charity in need.

- **Check On Your Peers!**: WorkPlus allows you to view your team members' daily steps and sleep hours from their Fitbit accounts.

- **Wellness Reminders**: WorkPlus displays you a carousel of facts, suggestions and reminders to keep you fit physically and mentally.


### Workplace Features

- **Chat Feature**: WorkPlus allows you to communicate with your colleagues in a real-time interactive chat window with the help of Django Channels & Sockets!

- **Add Project & Tasks**: WorkPlus allows you to add current and upcoming projects along with daily and unfinished tasks for everyone to see.

- **Upload Files**: WorkPlus allows you add files to the dashboard for everyone to see.

![image](https://user-images.githubusercontent.com/69211573/128547125-76965507-5090-4b9e-9038-0ce95378cd94.png)

![image](https://user-images.githubusercontent.com/69211573/128546682-8e2449cd-9ca9-4e9e-ad8d-bf1d55e571c5.png)

## How To Run Our Project:

1. Clone the entire repository.

2. Register a FitBit application at [https://dev.fitbit.com/login](https://dev.fitbit.com/apps/new) with the following details:

    **OAuth 2.0 Application Type:** Server
    
    **Redirect URL:** http://localhost:8000/fitbit
    
    **Default Access Type:** Read-Only	
    
    _**The other required fields are irrelevant to the process so please fill them in freely.**_
        
3. Add your registered application's **OAuth 2.0 Client ID** and **Client Secret** in [fitbit/fitbitvars.py](https://github.com/athu1248/WorkPlus/blob/8b3c05ee1ab7546e715e68f055126e4bfdea4f4b/fitbit/fitbitvars.py#L8-L9) where specified. **(Line 8 & 9)**
    
   Add your **OAuth 2.0 Client ID** to [templates/base1.html](https://github.com/athu1248/WorkPlus/blob/8b3c05ee1ab7546e715e68f055126e4bfdea4f4b/templates/base1.html#L83-L88) right after _client_id=_ in the href attribute. **(Line 88)**
	
4. Open your Terminal (Mac) and run the following lines of code:-


	Use appropriate command to navigate into the project directory: 
 
		cd WorkPlus	                #make sure you are in the right folder to begin with 	


	Activate a virtual environment (optional): 

		virtualenv env  
                     
		source env/bin/activate		#look for the path to your directory 

	
	Install all the required libraries and packages:
		
		pip install -r requirements.txt
			

	Run the server:

		python3 manage.py runserver   

## Why You May Be Unable To Run Our Project?
As stated in our sources above, our project uses Fitbit API to retrieve the user's daily activity. Doing so prompts us to apply our client_ID and client secret which is unique for every fitbit app. This is used to obtain the access token to activate the API. But since we are not dishing out any money to host the website on a paid server, the project will not work for anyone unless they have their own client_ID and client secret. We are looking forward to publishing our website online in the near future and hopefully store all our files on a designated hosting service.

## Languages Used:
- Python (Django)  	   
- HTML    
- CSS     
- JavaScript 

## Group Members
[Debashish Sahoo](https://github.com/debashish49) <br>
Atharva Kulkarni <br>
Darshan Shivakumar <br>
Aditya Sundar  

## Official Sources

- Fitbit API : https://dev.fitbit.com/build/reference/web-api/
- Bootstrap : https://getbootstrap.com/
- Trivia Questions : https://pastebin.com/QRGzxxEy

## License & Code Re-Use
The code for this project is released under the [GPL-3.0 License](./LICENSE). We ask that you please include a link back to this GitHub repository.
	 
![image](https://user-images.githubusercontent.com/69211573/128547156-c287ff4e-fefb-4bbc-8505-d222b1256a84.png)
