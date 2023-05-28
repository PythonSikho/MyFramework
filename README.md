# BDD Automation Framework v1.0 using Python

### How to set up
- Clone the project "git clone "https://github.hpe.com/hpe/BDD_Automation_Fw.git"
- Create virtual environment[Onetime] : `py -m venv venv`
- Switch to virtual environment       : `.\venv\Scripts\activate`
- Install packages: `pip install -r requirement.txt`


### How to execute

### sauceLab

##### By Tag Name:
- `python runner.py --module sauceLab --tags @Login`
- `python runner.py --module sauceLab --tags @invalidlogin`

##### By Feature Name:
- `python runner.py --module sauceLab --features login.feature`
- `python runner.py --module sauceLab --features login.feature,dashboard.feature`

##### By Module Name:
- `python runner.py --module sauceLab`


### Youtube

##### By Tag Name:
- `python runner.py --module youtube --tags @youtubeTest`

##### By Feature Name:
- `python runner.py --module youtube --features youtube.feature`

##### By Module Name:
- `python runner.py --module youtube`




 ##### Behave Command (sauceLab):


- `behave .//modules//sauceLab --tags=@validlogin -f allure_behave.formatter:AllureFormatter -o
  reports\BDDAutomation_23102022232145\results -D
  module=sauceLab -D job_id=BDDAutomation_23102022232145`

#### Links:

- GMAIL: `https://realpython.com/python-send-email/#:~:text=Set%20up%20a%20secure%20connection,attachments%20using%20the%20email%20package`
- CURl: `https://curl.se/windows/`
- Allure: `https://github.com/allure-framework/allure2/releases`
- Netlify API: `https://docs.netlify.com/api/get-started/`
               `https://docs.netlify.com/api/get-started/#zip-file-method`
- Git Exe: `https://git-scm.com/downloads`




#### Git commands-
- To clone the project: `git clone git@github.com:PythonSikho/MyFramework.git`

- `git status`
- `git add .`
- `git commit -m "My firts code push"`
- `git push origin main`

- To have the latest code - `git pull`

#### Jenkins Allure Support
##### Open Console/Command line --> Go to your Jenkins installation directory (very likely cd "C:\Program Files\Jenkins\"). 
- Execute the following commands respectively:

To stop:
`.\jenkins.exe stop`

to start:
`.\jenkins.exe start`

to restart:
`.\jenkins.exe restart`

### Plugin required:
- `Parameter Separator Plugin`
- `Allure Jenkins Plugin`

### Global Tool Configuration
- ALLURE_HOME - `C:\allure-2.22.0\allure-2.22.0`
- JAVA_HOME - `C:\Program Files\Java\jdk-11`

### Build-in Node
- label - master
- Number of executors - 10
