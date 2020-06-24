# Basics 
Version control is required to enable users to collaborate effectively on software engineering projects. In this series of workshops , we will be looking at Git , a version control system designed by Linus Torvalds (yes that guy who created Linux). We will be looking at an extremely basic idea of how to use Git (without going into the nitty-gritty stuff) in this workshop.

# Prerequisites
1. This workshop is intended to take around an hour.
2. You need Internet access.
2. Make sure you have a GitHub ID before starting this workshop otherwise you wouldn't be able to complete it.
3. Make sure you have a device with some operating system ( Android and DOS do not count) , preferably Linux.

# Git Installation
1. [Download Git for your specific operating system by clicking this link](https://git-scm.com/downloads)
2. Check your version installed using ``` git --version ```
3. Configure your Git username and email ( associated with commits you will make) using 
```
git config --global user.name "<Your GitHub username>"
git config --global user.email "<The email address you registered with your GitHub account>" 
```

# Cloning this project 
1. Login via GitHub and navigate to [this project](https://github.com/Maths-Coding-Society/Introduction-to-Git) .
2. Click the <b>Fork</b> button on the upper right corner. This will create a copy of this project under your GitHub ID. DO NOT CLONE THIS PROJECT. 
3. Once forked go to ```<your-Github-username>/Introduction-to-Git ``` and then click clone. There will be a url of the form ``` https://github.com/<your-Github-username>/Introduction-to-Git.git ``` (Make sure to fork this repository first and substitute your correct GitHub Username). Copy this URL.
4. Go to your terminal , navigate to a suitable folder and then type ``` git clone https://github.com/<your-Github-username>/Introduction-to-Git.git```. This step clones (aka creates a local copy of the repository on your local system) the repository.

# Making Commits 
1. Type ```cd Introduction-to-Git ``` to enter the directory. Then type ```cd sandbox ``` to navigate to the Sandbox directory where we will be doing all of the stuff for our workshop.
2. Type ``` nano add.txt``` . A window will open with the text editor <b>nano</b> . Just type ```Use git add to add files```. Press ```Ctrl + X ``` to exit , ``` Y ``` to save the file and then ```Enter``` to confirm it. 
3. Type  ```cd ..```  - this will take you to the parent directory of ```sandbox``` which is ```Introduction-to-Git```.
4. Then type 
```
git add sandbox/add.txt
git rm sandbox/remove.txt
``` 
This will add the file ```sandbox/add.txt``` and remove the file ```sandbox/remove.txt``` from the repository commit.

5. Type ```git commit -m "<some commit message which you find suitable"``` . Make sure that you replace the placeholder with a 'suitable and descriptive' message.
6. Type ```git push``` . This will push your code to GitHub (this is because GitHub is set as a remote origin for push and pull , more on that in subsequent workshops). You will be required to enter your GitHub username and password. You will see some message that some objects are being pushed to GitHub. If you now go to GitHub you will see that the ```remove.txt``` file does not exist anymore and there is an ```add.txt``` file instead of it , which we pushed from our local machine. 
7. Now click on ```add.txt``` and open it in GitHub's online editor ( click the small pencil towards the upper-right). Add the text ```Hurrah I know the basics of git``` to it and commit.
8. Now go back to the command line (inside the Introduction-to-Git folder) and type ```git pull```.  You will see that the changes you made on the online GitHub editor are now visible in your local copy of the repository.

# Conclusion
Congratulations! You now know the basics of Git. Thank you for reaching the end of this workshop.</br>
We hope you will complete our subsequent workshops. - RG

# Bonus Material
Check out [this project on Repl.it](https://repl.it/@rkclg/MathsCodingSocietyBonusMaterial#main.py) . Experiment and try coming up with more vector functions !
 
