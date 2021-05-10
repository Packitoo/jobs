# We are Packitoo (Pack-It-Too)

At Packitoo, we made the first marketplace for packaging (https://marketplace.packitoo.com/) and the first instant pricing engine or the packaging industry "HIPE" (https://hipe.packitoo.com/), **making prices in seconds instead of days or weeks** like this industry is used to.<br/>
We have big projects, tons of new features to make on a high quality react app, with a node backend and a python microservice for price prediction.
We are animated by the following values:

* PASSION: We like what we do, it drives us to make an awesome app
* RESPECT: We are all different, with our strengths and weaknesasses. We respect our customers, our colleagues, our planet and everyone on it. Acting with Kindness ("bienveillance" in French) is the mindset, because people dont make mistakes on purpose
* EXPLORATION: We are sailing in unchartered waters, connecting customers and manufacturers withg a software that changes completely the way they work

# The job

We are looking for a **senior web developer**

* Mainly **python** development but not exclusively
* Including handling the devops for his/her work
* From the stories described in our backlog (by the Product Manager, by you, by the team), you share your plan to implement (architecture level, code, test, ops...)  and proceed on making a merge request for the team to comment on
* Keep the python stack performance in check
* Review peers merge requests
* Willing to pair program and remote pair programming (to learn from others, to learn to others, to keep the story in the scope, etc.)
* Work in 3 weeks sprints, with retrospectives, we have been using sprint velocity for quite some time and we are happy with it.
* Be part of the morning stand ups with all the team. Outside of that, we try to keep the fewest meetings possible, leaving people to have focus hours.

# Requirements

* 2 years with Python with a **framework such as Flask or Django, an ORM, microservices, API, testing** (pytest or others)
* Experience choosing and setting up a proper dev environment and practice (lint, test, building...)
* Experience with **development patterns** (MVC, Clean architecture, Hexagonal...)
* you are carefull about code organisation and seperation of concerns, proficient using recursivity, polymorphism, exception management, package management, import structuring,
* Experience debugging production issues, alert and log management
* Familiar with docker and an orchestration tool (swarm, kubernetes...), postgresql and debugging docker/ops issues
* Knowledge of CI/CD with Gitlab, linux system administration, firewall, ovh, shell, variable scoping
* Willingness to pickup basic knowledge of a new tech for testing, CI/CD
* You are an eternal student

# Bonus points

* You have worked in a startup, you like working in teams, pair programming, coaching juniors
* You are passionate about softwares, computers, technology and know all the little parts that make Internet
* You have experience in Typescript (React / Node) or Ruby (Rails) or **machine learning** tools and DataFrame usage
* You are familiar with the british comedy group that inspired python's name
* You speak **French**
* You use VSCode and liveshare

# Location and details

* R&D Team is **remote** since the beginning (Pau, Bordeaux, Bergerac, Villasavary, Beziers)
* We meet **once a month at the office in [Pau](https://en.wikipedia.org/wiki/Pau,_Pyr%C3%A9n%C3%A9es-Atlantiques)** (#gastronomie #ski-slopes-in-60mins #ocean-in-80mins)
* You will have to live in reasonnable distance from Pau to come over once a month for 3-4 days (so it's about 80% of the time remote)

# Hiring process

1. Send your resume with a letter explaining what you are looking for
2. We review your application
3. We call you for a 15 min to check general informations and clear out process
4. Possibly a tech challenge if you dont have code to show
5. Tech interview about challenge or remote pair-programming
6. Culture-Fit interview (can happen before the tech interview)
7. We send you a contract offer
8. Win

Please send us an email at jobs@packitoo.com

```python
from datetime import timedelta, time, date

class SeniorWebDeveloper:
    def __init__(self, candidate):
        position: 'Python Devops'
        company:{
            "size": 10,
            "location" : "Pau",
            "counttry": "France",
            "founded": date(2017, 7, 15),
            "language": [French, English],
            "members": {
                "PO": 1,
                "UX": 1,
                "DEV (inc CTO)": 3,
                "GROWTH (CMO)": 2,
                "SALES (COO)": 1,
                "CEO": 1,
                "CUST_PROJ_MANAGERS": 2
            },
            'softwareWebsite': 'https://hipe.packitoo.com/',
            'serviceWebsite': 'https://www.packitoo.com/',
            'tech_stack': 'https://stackshare.io/packitoo/hipe/main'
        }
        current_technologies: [Flask, Shell, Make, DockerSwarm, Ubuntu, Nginx, Pip, Virtualenv, PostgreSQL, API, gitlab-CI]
        other_technologies: [nodejs, typescript, react, redux, redux-saga, material-ui, DataFrames, Scikit, OpenAPI, ssh, tmux]
        remote = '80%'
        startup = True
        automated_testing = True
        cicd = True
        specs = True
        code_reviews = True
        pairing = True
        retrospectives = True
        sprint_lenght_in_weeks = 3
        other_tools = ['Zoom', 'Fibery', 'Figma', 'Git']
        morning_stand_up = time(hour=9)
        focus_ours = True
        team_diner_and_drinks = True
        french_contract_type = "Cadre"
        french_standard_benefits = ['medical', 'holidays', 'rtt']
        if candidate.location == 'Pau':
            unlimited_coffee = True
            desk = True
            colleagues = True
        elif (candidate.comute_time_to_pau() < timedelta(hours=4)):
            trip_to_pau_frequency = 'once_per_month'
```
