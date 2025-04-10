

# IFocusAWSDevOps

24/02/2025::
==============

What is Git?

Git is a free, open-source version control system (VCS) that helps developers manage their code. It's the most widely used tool VCS(version control system)
Git is fast for committing, branching, merging, and comparing past versions
Git is very high Performance and Flexibility,Security 

Install Git on windows:: go to below url and download 64-bit Git for Windows Setup.

https://git-scm.com/downloads/win

After download double click on Git-2.48.1-64-bit.exe file , git will be install Successfully

GitHub account creation:: for creating github account EmailId is Required

go to link --https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home

Enter Email & password ,Username click continue ---Account will create successfully
![image](https://github.com/user-attachments/assets/f108ebee-716b-43d8-b5b5-d19ed291e9c1)

Github::Github is a one of the SCM(Source code management) tool and store the Project code.

Repository: storage area of your source code.
Create a Repository on GitHub

click Repositories

![image](https://github.com/user-attachments/assets/904ece7c-23f4-475c-9a6c-e7eb0ccd5e19)

Click New

![image](https://github.com/user-attachments/assets/aefd6151-23b8-4b65-9089-d7412adbb8dc)


Enter Repository Name::

![image](https://github.com/user-attachments/assets/872899bf-bcec-468e-b1c6-023044f49df4)



Public::
Anyone on the internet can see this repository.

Private::
You choose who can see and commit to this repository.

Click Create Repository


![image](https://github.com/user-attachments/assets/0f6d5004-1523-4e33-86c0-41640e7b279e)

Repository Created SUccessfully with Default branch main

![image](https://github.com/user-attachments/assets/e4f9f53d-91e2-4ce0-bc86-b152aa322e66)

Push Sample Java Code To Github Repository::

https://github.com/spring-projects/spring-petclinic

Fork::Fork means to make a copy of the repository into my own github account
A fork is a copy of a repository

![image](https://github.com/user-attachments/assets/9710696d-1991-4f8d-a66c-bc4ed70d44c3)

Fork done

![image](https://github.com/user-attachments/assets/9d7eeeeb-adb0-4aff-a5a4-78755e99d1c7)

Clone Project and Push Changes to Github Repository::

Go to Code and copy url

![image](https://github.com/user-attachments/assets/cfe0f9a6-e661-4a4c-871f-7a6d84c97f9a)

Go to Local Folder and right click and Open Git Bash here and it will navigate to gitbash

![image](https://github.com/user-attachments/assets/8622a586-526f-41c6-bb5c-3494372e0007)

navigate to gitbash

![image](https://github.com/user-attachments/assets/6a8aab98-73eb-4fc8-bfb2-607297064e75)

Copy Repository URL

![image](https://github.com/user-attachments/assets/19aedccf-571e-4034-b5fc-8d05d442f39d)

Git Commands::

>git clone <repo url>
>git clone https://github.com/parasa7358/spring-petclinic.git
>
>![image](https://github.com/user-attachments/assets/e8b7464b-069e-43ed-b372-86ddd7a730c4)

![image](https://github.com/user-attachments/assets/0590c587-3511-4a80-9de1-52536ec90cef)

>cd <reponame>
>git checkout <branchname>
>git status
>git add --all
>git status
>git commit -m "commit message"
>git push origin
>git pull
>git add .

All Steps::

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS
$ git clone git@github.com:parasa7358/spring-petclinic.git
Cloning into 'spring-petclinic'...
The authenticity of host 'github.com (20.207.73.82)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
remote: Enumerating objects: 10425, done.
remote: Counting objects: 100% (2/2), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 10425 (delta 0), reused 0 (delta 0), pack-reused 10423 (from 2)
Receiving objects: 100% (10425/10425), 7.67 MiB | 706.00 KiB/s, done.
Resolving deltas: 100% (3935/3935), done.

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS
$ cd spring-petclinic/

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (main)
$ git checkout feature/2025.02.24
branch 'feature/2025.02.24' set up to track 'origin/feature/2025.02.24'.
Switched to a new branch 'feature/2025.02.24'

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (feature/2025.02.24)
$ git status
On branch feature/2025.02.24
Your branch is up to date with 'origin/feature/2025.02.24'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   pom.xml

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (feature/2025.02.24)
$ git add --all

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (feature/2025.02.24)
$ git commit -m "This is first commit for this project and updated pom.xml"
[feature/2025.02.24 434fce4] This is first commit for this project and updated pom.xml
 1 file changed, 1 insertion(+)

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (feature/2025.02.24)
$ git push
ssh: Could not resolve hostname github.com: Name or service not known
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (feature/2025.02.24)
$ git push origin
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 338 bytes | 338.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:parasa7358/spring-petclinic.git
   6c05fc9..434fce4  feature/2025.02.24 -> feature/2025.02.24

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/Ifocus/AWS/spring-petclinic (feature/2025.02.24)
$

Screenshot::

![image](https://github.com/user-attachments/assets/1e723036-90a9-4cee-8d31-2746f37f525b)


25/02/2025:::
==============

Github branching strategy::


![image](https://github.com/user-attachments/assets/dac55b58-d16d-4049-8a2b-4c3a8f979999)

main or master branch:: This is default branch and whenever we created the empty Repository by defauly main or master branche is created automatically.
main or master branch always stable and live code 

feature branch:: It could be a new feature, an improvement of existing features, bug fixes, or any other changes. A feature branch is a type of branch in Git typically used to develop new features for the software.feature branch will created from main or master OR feature branch created from latest release branch always based on the release cycle

formate:: feature/YYYY.MM.DD
 feature/2025.02.24

release branch:: Based on the release we have created release branch accourdingly and starts the next release cycle.
always release branch created from master only and master have stable and live code and post release we shold merged code changes to master branch only

release/2025.02.24

hotfix branch:: always created from main or master branch only for production fixes.once production fix done we should merged directly to main or master branch only.

always created this hotfix branch for production issues fixes

bugfix:: this branch is created from release branch to fix the LLE(lower level environemnt)/Pre-Prod/UAT/Non-Prod issues and once LLE issues fixed ,we should pushed their changes to release branch only.

cloning references::

![image](https://github.com/user-attachments/assets/87f6ed4a-095b-4faa-854a-7fcdc019f31f)


Generate SSHKeys::

syntax::ssh-keygen -t ed25519 -C "your_email@example.com"

Keys avaibale path and save the key (/c/Users/HP/.ssh/id_ed25519):
![image](https://github.com/user-attachments/assets/c1031abb-57bf-4585-88a9-e1fbb9358621)

![image](https://github.com/user-attachments/assets/ce78114d-1a3f-4adf-a677-c3f26736f6cc)


Please follow below links for more understanding 

https://docs.github.com/en/authentication/connecting-to-github-with-ssh

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

Once genearted the keys (public/private) and copy public key to Github Account

Go to -->settings

![image](https://github.com/user-attachments/assets/e6856f23-6d62-4e02-8fb2-05c720542ec3)

Click SSH and GPG Keys

![image](https://github.com/user-attachments/assets/906f1f68-79a8-4920-837f-38f165e5849e)

click New SSH Key

![image](https://github.com/user-attachments/assets/a461189f-f9e1-415c-b52e-c25f6cfaf1d2)

Add new SSH Key and click Add SSH Key

![image](https://github.com/user-attachments/assets/f62d4d90-f588-462b-bf04-54de51e566d8)


Raise PR (Pull Request) :: Merge the code from one branch to another branch that is called pull request

below are the steps to raise PR::

Go to -->Pull requests and click

![image](https://github.com/user-attachments/assets/5cfe4883-dd46-4643-a506-b54262c36202)

Click New Pull Request::

![image](https://github.com/user-attachments/assets/37020743-a2e9-4163-9afd-7680d58fc63a)

![image](https://github.com/user-attachments/assets/dad8eec2-b480-460f-8715-9d9c5fc3c12d)

please select base & compare branches so here base branch is release/2025.02.25 and compare branch is feature/2025.02.25

i'm going to merge code changes from feature branch to release branch 

![image](https://github.com/user-attachments/assets/185f0572-c51a-4ab2-884c-d2694522b268)

click create pull request

![image](https://github.com/user-attachments/assets/91068166-9d06-4b47-9d68-8c1251b0872f)

![image](https://github.com/user-attachments/assets/08a98671-c810-46fc-9024-17bae7538a61)


parasa7358 wants to merge 1 commit into release/2025.02.25 from feature/2025.02.25  

click merge request

![image](https://github.com/user-attachments/assets/44a4b84e-1aef-4b19-a93e-64e48b362b29)


confirm merge

![image](https://github.com/user-attachments/assets/cc12b687-b664-4497-bf91-0ab17f37bfa0)

Merged

![image](https://github.com/user-attachments/assets/9ee86d60-3e25-40a2-8d45-3bfe67668a2e)


26/02/2025::
=============

1. completely we have occupied this session is issues resolutions and we will continue new topic in next session


27/02/2025::
============

If multiple developers OR DevOps Engineers are working on same Project/MOdules, if they tried to commits thier code changes to Repository, it will faces the  conflicts issues and how to resolved those conflicts issues in real time projects 


![image](https://github.com/user-attachments/assets/8bc72ca5-a9fd-407b-9d37-48824e5375b7)

Avoide conflicts:: Before pushing the code changes to github repository, make sure, you should be run the command -->git pull

>git pull --->git pull command is use, copies changes from a remote repository directly into your working directory (local directory) and merged code changes from remote repository to local repository 
>git fetch ---->The git fetch command only fetch the changes into your local Git repo and it will not merged anything. just fetch the details

Please create A,B,C directories in your local machine and clone the project code separately 

![image](https://github.com/user-attachments/assets/7e786310-5092-4975-9eb9-7b18801353d8)

Editor steps for Resolved the conflicts::

editor::

1.press i from your keyboard, INCERT
2.press the esc from your keyboard at top left corner 
3.shift+: 
4.wq


User -A Activity::

 git checkout feature/2025.02.27
error: pathspec 'feature/2025.02.27' did not match any file(s) known to git

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (main)
$ git pull
From github.com:parasa7358/spring-petclinic
 * [new branch]      feature/2025.02.27 -> origin/feature/2025.02.27
Already up to date.

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (main)
$ git checkout feature/2025.02.27
branch 'feature/2025.02.27' set up to track 'origin/feature/2025.02.27'.
Switched to a new branch 'feature/2025.02.27'

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (feature/2025.02.27)
$ git status
On branch feature/2025.02.27
Your branch is up to date with 'origin/feature/2025.02.27'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Jenkinsfile

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (feature/2025.02.27)
$ git add --all
warning: in the working copy of 'Jenkinsfile', LF will be replaced by CRLF the next time Git touches it

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (feature/2025.02.27)
$ git status
On branch feature/2025.02.27
Your branch is up to date with 'origin/feature/2025.02.27'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Jenkinsfile


HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (feature/2025.02.27)
$ git commit -m "Added jenkins file for Feb Release"
[feature/2025.02.27 9ad4ee0] Added jenkins file for Feb Release
 1 file changed, 22 insertions(+)
 create mode 100644 Jenkinsfile

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (feature/2025.02.27)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 483 bytes | 241.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:parasa7358/spring-petclinic.git
   e4b9aa2..9ad4ee0  feature/2025.02.27 -> feature/2025.02.27

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/A/spring-petclinic (feature/2025.02.27)
$

User-B Activity::

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/B/spring-petclinic (feature/2025.02.27)
$ git pull
Already up to date.

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/B/spring-petclinic (feature/2025.02.27)
$ git status
On branch feature/2025.02.27
Your branch is ahead of 'origin/feature/2025.02.27' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/B/spring-petclinic (feature/2025.02.27)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 586 bytes | 293.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To github.com:parasa7358/spring-petclinic.git
   9ad4ee0..ed57c5e  feature/2025.02.27 -> feature/2025.02.27


User-C Activity::

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/C/spring-petclinic (feature/2025.02.27)
$ git status
On branch feature/2025.02.27
Your branch is ahead of 'origin/feature/2025.02.27' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

HP@DESKTOP-E518Q66 MINGW64 ~/Desktop/C/spring-petclinic (feature/2025.02.27)
$ git push
Enumerating objects: 33, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (13/13), 1.14 KiB | 233.00 KiB/s, done.
Total 13 (delta 5), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (5/5), completed with 5 local objects.
To github.com:parasa7358/spring-petclinic.git
   ed57c5e..80681f1  feature


   Please be practice above 3 users activity in real time bases 

   
28/02/2025::
================

Jenkins Introductiion::

Jenkins is a free and open source automation server/tool. It helps automate the parts of software development related to building, testing, and deploying, facilitating continuous integration and continuous delivery.

<img width="846" alt="jenkins overview" src="https://github.com/user-attachments/assets/ffb9a0c8-0a8c-4b43-953e-36cd17297716" />

Jenkins is a Orchestration tool

Jenkins is a CI/CD tool

Jenkins is a Schedular

Jenkins is a crone job schedular 


Continuous Integration(CI)::the practice of automating the integration of code changes from multiple Developers into a single software project. It's a primary DevOps best practice, allowing developers to frequently merge code changes into a central repository,after which automated builds and tests are run automatically.

developers frequently commit to a shared repository using a version control system such as Git,A continuous integration automatically builds and runs unit tests on the new code changes to immediately using jenkins Orchestration.

Continuous Delivery (CD)::Continuous Delivery is a software development practice in which code changes are automatically built, tested, and prepared for release to production in a consistent and reliable manner. The key distinction of continuous delivery is that the process of deploying the code to production is done manually by a human decision-maker.

![image](https://github.com/user-attachments/assets/a3be0abd-12cf-49a5-b1e5-e56d54ac1080)



Continuous Deployment(CD) :: Continuous Deployment is an extension of continuous delivery. With continuous deployment, every change that passes through the automated tests and builds is automatically deployed to production without any human intervention. The deployment process is fully automated.

![image](https://github.com/user-attachments/assets/03cd5335-7656-4b39-80c3-e7ba7a0234a9)


Roles And Responsibilities::

1)The devops engineer was responsibility to release the product to the market as soon as possible
2)release the product speed to the market
3)Devops engineer was give continues feedback to the developers
4) Devops engineer responsibility start from git and end with production

A) when your activity start from git and end with production environment(production servers)Continues deployment
when your activity start from git to LLE(lower level environment,testing environment,pre-prod…et) environment(pre-production servers)Continues delivery non-production environment

Download JDK 17 ::

https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html

Windows x64 Installer	153.92 MB	
https://download.oracle.com/java/17/archive/jdk-17.0.12_windows-x64_bin.exe (sha256 )

OR

Windows x64 Compressed Archive	172.87 MB	
https://download.oracle.com/java/17/archive/jdk-17.0.12_windows-x64_bin.zip (sha256 )

Download Maven::

https://maven.apache.org/download.cgi

Source zip archive	apache-maven-3.9.9-src.zip

01/03/2025::
==================

JDK 17 Environment setup::

Go to Search box & type Edit the system environemnt variables and click


![image](https://github.com/user-attachments/assets/66f98991-dc2a-4bd5-a093-67b88997e851)

It will navigate to System properties 

![image](https://github.com/user-attachments/assets/2b14fcee-1b5d-4f00-ac6e-b0ee83932384)

Open Environemnt Variables

![image](https://github.com/user-attachments/assets/5c2b431e-caa8-4a64-86ed-71f379f57c7b)

![image](https://github.com/user-attachments/assets/b3e2a06a-27ec-46a2-b1ac-8579c5be9321)


User variables::
JAVA_HOME=C:\Users\HP\Downloads\jdk-17.0.12_windows-x64_bin\jdk-17.0.12
 
![image](https://github.com/user-attachments/assets/8ad54751-f25d-4a0c-9339-1e90caa81094)

System variable::

%JAVA_HOME%\bin
%MAVEN_HOME%\bin
 
![image](https://github.com/user-attachments/assets/00ace73f-2dad-442d-9404-7ade62e0ba70)

![image](https://github.com/user-attachments/assets/14ea70d3-2d24-4f7d-a752-c412d4fb704d)


Maven setup::
MAVEN_HOME=C:\Users\HP\Downloads\apache-maven-3.9.9-bin\apache-maven-3.9.9

![image](https://github.com/user-attachments/assets/8a0f15af-32c5-4624-af43-59959b02e8c8)

Download link
https://maven.apache.org/download.cgi


Make sure we should setup the path at system variable 

JAVA_HOME & MAVEN_HOME

![image](https://github.com/user-attachments/assets/07ddf2ff-a7f1-470b-b07c-66316e8b1d7e)


now verify the java version & maven version:: go to git bash and verify. below are refreenced screenshots

> java -version

![image](https://github.com/user-attachments/assets/4319ddcf-5a6a-4844-aa74-5e7e3b88d601)

> mvn -v

![image](https://github.com/user-attachments/assets/ff578d8a-5c15-4686-8fdf-d9c94240ee73)


once above setup is ready then we will proceed to installe jenkins 

02/03/2025::
====================

Installed jenkins in Windows::
https://www.jenkins.io/download/

Go to google search -->download jenkins war file for windows

![image](https://github.com/user-attachments/assets/d5550fe2-9af0-4376-af1b-6d4056beafe8)

Click --->WAR file link


![image](https://github.com/user-attachments/assets/3504e05f-6c0d-47a8-9b51-dffbcd0f790f)

Please follow the below link steps to installed jenkins in your windows machines

https://www.jenkins.io/doc/book/installing/war-file/

Steps::

https://www.jenkins.io/download/
1. First download the jenkins.war file and right click -->open gitbash here
2. run the command  -->java -jar jenkins.war --httpPort=9090

![image](https://github.com/user-attachments/assets/1cf75767-d6d7-4dfb-9a75-ccb9365b5ffb)

Browse to http://localhost:9090 and wait until the Unlock Jenkins page appears

Installed the default suggested plugins

![image](https://github.com/user-attachments/assets/081c44fc-a6a3-46fa-82e3-7b34c2dc2dd6)

click on continue 

Need to create jenkins user profile 

USER Name--->admin (any name you can provide)
PASSWORD  -->admin  (any password as your wish but make sure you should remembered the these credentials)

![image](https://github.com/user-attachments/assets/f0458a88-da81-4d32-9f87-42458fd214a1)


Create sample Freestyle project::

Click New Item

![image](https://github.com/user-attachments/assets/d9e7f707-aa00-4c74-b9ca-30489ded6f55)


Configuration stages::

1.General

2.Source code management (SCM)

3.Triggres

4.Environment

5.Build Steps

6.Post Build Actions


![image](https://github.com/user-attachments/assets/b7b5caf1-3d81-4de0-aebc-c2dc5080f916)


General Section provide the Project/job description 


At SCM stage level select the Git and provide the github details

![image](https://github.com/user-attachments/assets/827c5b34-8a6e-41ad-b6e1-4899348730d6)

Branches to build

![image](https://github.com/user-attachments/assets/51cf678c-afbd-40bc-bbb5-fae55e4c5537)

Poll SCM:: i want triggered the jenkins job build every minute

![image](https://github.com/user-attachments/assets/7bab6e2d-7868-460e-bd42-b2697195f3fe)

Build steps::select the Invoke top-level Maven targets
Goals section
>mvn clean install

Maven goals::

>mvn test

>mvn install


>mvn clean install


>mvn clean


>mvn package

![image](https://github.com/user-attachments/assets/53d49170-9dfe-4cad-abc0-50bf268e96c7)


Job will be created

Click Build Now


Buils is Inprogress

![image](https://github.com/user-attachments/assets/c6e399ce-ac52-47de-94a3-b4d6d156dce5)





03/03/2025::
=====================


Poll SCM ::Jenkins server ask git if there is any changes in git server or not, if changes there Jenkins server build/package the changes , every change build happened like 5 mints ,means every 5 minutes verify the Jenkins server to git if there is any changes 

![image](https://github.com/user-attachments/assets/6f436ad6-e92a-40e3-831a-23219c288217)

POLL SCM ----* * * * * --every minute when every commit 

Build Periodically :::something changes in git I want build the changes, what can you do for that,
For example –I want build every 24 hr ,so only 24 hrs only build happened.

Create one sample POLL SCM jenkins job::
===========================================
Go to jenkins Dashboard
click New Item

![image](https://github.com/user-attachments/assets/1c62657f-935b-4eed-b032-08842fb09a57)

Description

![image](https://github.com/user-attachments/assets/3a54ba69-b2aa-4443-ad9b-d18ab5fbde02)


Provide the Git URL

![image](https://github.com/user-attachments/assets/1fb7b83f-3bba-411b-aad9-a725f25d3e1c)


Branch buiild

![image](https://github.com/user-attachments/assets/71aec8f1-4783-4e97-97cb-232dd18811ae)

POLL SCM:: * * * * *

every minute build was trigger when new commits happend in github repository

![image](https://github.com/user-attachments/assets/d6ab7a34-156a-4430-9d40-31e362ad23b1)


Build Steps::

![image](https://github.com/user-attachments/assets/4aae78af-d217-41de-a1e6-16bfe2e34472)


Build Periodically:::	H/15 * * * *   ----this build happened every 5 minutes without commits ,if changes are commit or not but every 5 mints build happened in Jenkins 

Create Sample Build peridiocally jenkins job::
=============================================

Description

![image](https://github.com/user-attachments/assets/5ad69478-039e-4ef7-a35f-cb18ed8364f1)

Git url::

![image](https://github.com/user-attachments/assets/b2cbdb7c-14ac-4fae-a240-90cc7a82c78d)

Build the branch

![image](https://github.com/user-attachments/assets/94230c57-b88f-4ab1-b894-151f30fa6d53)

every 5 mints build will trigger

Build Periodically:::	H/15 * * * *   ----this build happened every 5 minutes without commits ,if changes are commit or not but every 5 mints build happened in Jenkins 
![image](https://github.com/user-attachments/assets/a5321109-944b-4e79-9294-e28c2adfea0d)

click save 

Whenever you configure a build activities :::
=======================================

SCM::

	Where is your project

Build environment::

---all about your workspace folders 

Build Triggers::

--whenever code changes 
--periodic
---script calls 

Build steps::

Dev team will tell ,

Post build::

That aim is giving continue feedback to dev team

--send mails
--build pass/fail
--CI

Manage Jenkins::
=================

1.configure system

--number of executors
--E-mail notifications
--internall org SMTP

We don’t change anything in system level configurations

Configure Global security::
=========================

--matrix security
---jenkins level security

Configure credentials::
===============

Above options we can’t do anything in your organization


Global tool configuration:
================

Java::

![image](https://github.com/user-attachments/assets/64a43077-1689-4802-9fab-d316634d426d)

 

Maven::

![image](https://github.com/user-attachments/assets/74bac0fa-9552-4289-b1db-79f729b9de75)

 
Plugins::
===

Manage jenkins --->plugins


Availabe plugins 
Installed plugins

![image](https://github.com/user-attachments/assets/b1f32f0a-68e2-4bc1-b521-7f67f9bd9956)


if you want installe new plugin ::

Go to Availabe plugins and erach plugins name

![image](https://github.com/user-attachments/assets/5e17685a-430d-437a-99b3-a29370b374cc)

Once insatlled the plugin we will get the UI(User Interface) and it will not installed any software just get the UI

04/03/2025::
=============

crone job formate link

https://crontab.guru/examples.html

Parameterized Jenkins Jobs ::

Run the same job with different inputs without modifying the configuration manually

Go To New Item

![image](https://github.com/user-attachments/assets/20b1237b-1681-4e77-ad8b-33ee8ac69b97)

Enter Job Name, Free style project and click ok

![image](https://github.com/user-attachments/assets/106bb57e-5466-4e1d-9ead-c977aaac60e7)


Enter the description

![image](https://github.com/user-attachments/assets/4944c35f-86db-42a4-8bb8-4b3d9987fd81)

Select the option This project is parameterised

![image](https://github.com/user-attachments/assets/4eeab439-3e45-4320-a7de-73360c28c3c3)

Click Add Parameter

![image](https://github.com/user-attachments/assets/3570dcc9-72a0-4034-8da3-1a70e0341fa7)

Select optiions String parameter or choise parameter or boolean parameter you can select the ny options based on your requirement 

![image](https://github.com/user-attachments/assets/210ae086-fecf-42b2-9322-966b85431d18)

select string parameter

![image](https://github.com/user-attachments/assets/aa0b6706-bda8-4de8-a094-d14e4955fc34)

Select Choise Parameter

![image](https://github.com/user-attachments/assets/48baed03-fe9c-482b-870b-ba4126eb2b4a)

choise parameter

![image](https://github.com/user-attachments/assets/a50a06a9-5063-4f12-8d10-0f44ee473f46)

Click Save

You Can observed this project is parameterized 

![image](https://github.com/user-attachments/assets/05be584b-bd82-4f00-89c7-6358a4ca5ca4)

Click Build with parameter

![image](https://github.com/user-attachments/assets/a7317486-0b18-4e78-9a64-4113f712a757)

select deployment environment

![image](https://github.com/user-attachments/assets/b12a618f-a8da-4c8f-b19c-7b92af2431da)

select which versioj you want to deployment like tis you can configured real time parameterized project in jenkins

![image](https://github.com/user-attachments/assets/33a52ced-4fa7-4b69-a0f9-a82fe436cdfd)

Click Build

![image](https://github.com/user-attachments/assets/7acf8c06-b734-4512-acf7-86ed9fd9053a)

![image](https://github.com/user-attachments/assets/1cec807a-76cc-4446-a589-4767563b90eb)

I want Build a 3 projects ::
===========================

![image](https://github.com/user-attachments/assets/a3c32e99-2361-4462-a7bc-dfa05310191d)

Project-A,Projec -B,Projec - C 

Projec A is  (Downstream project is ---Projec B)

Projec B is (UP Stream project for ----Projec A)

Projec C is (downstream project --Projec B)

i created 3 free style project in jenkins 

Project-A ::
==============

Github URL::: https://github.com/parasa7358/spring-petclinic.git

![image](https://github.com/user-attachments/assets/e8073061-b815-4945-bd7f-c20b3a6576e2)

Post Build Action , select the option Build Other Project  Project-B

![image](https://github.com/user-attachments/assets/ef75f777-c273-4255-b063-f9853072dfcb)

Project -B ::
=============

Github URL:::https://github.com/parasa7358/onlinebookstore.git

![image](https://github.com/user-attachments/assets/2ee62e92-e677-4717-93be-77d6dd1ecbf9)

Post Build Action , select the option Build Other Project Project-C

![image](https://github.com/user-attachments/assets/ec7cfc18-002b-4dc3-8438-a75b12b9a438)


Project-C::
============


Github URL:::https://github.com/parasa7358/game-of-life.git

Discard old builds:::
====================

Days to keep builds---->give 15
Max # of builds to keep ==give 10

![image](https://github.com/user-attachments/assets/58a96f10-ff53-4306-a5a7-dd20b42e1c9f)


5/03/2025::
============

Post build Action i want to published artifacts & test results

![image](https://github.com/user-attachments/assets/fcd3ea28-a352-431f-8e1b-86758787fe7a)

I'm going to created one free style job and configured Post-build Actions

In post build Action select the option Archive the artifacts

>target/*.war

![image](https://github.com/user-attachments/assets/39dcf26d-74ee-4c7f-bc28-bb7f6116fedb)

In post build Action select the option Publish JUnit test result report for to published the test results

>target/surefire-reports/*.xml


![image](https://github.com/user-attachments/assets/e04f371d-b684-406b-9210-50fb74b6ea79)

Execute the Jobs in Parallel::
==============================


1.By Default execute the Jenkins build jobs are sequence way,one by one 

2.Don’t do 2 projects build parallel  this is real time scenario but we can do parallel builds as well one job

Jenkins build parallel setup
Go job ---> configure ----> Generall ---> Execute concurrent builds if necessary



![image](https://github.com/user-attachments/assets/909edd87-548d-4ded-a862-29cf850fac05)


Here 5 builds execute parallel ,I kept executor is 5 this is same machine 

![image](https://github.com/user-attachments/assets/a840a224-5cbb-43cc-92c1-d135db4ce00f)

I want to show test results ::
=================================


>ls target 

Post build action stage

Select archive the artifact
--target/*.jar

Junit test results::
--target/surefire-reports/*.xml


See test results & antifactory ::
===================================

![image](https://github.com/user-attachments/assets/2711b453-072e-40d2-9596-afce8f586310)


3.For every company will do sequence build on one project this is recommended approach

Please read and understand the below important point for parallel execuion job::
==================================================================================

When this option is checked, multiple builds of this project may be executed in parallel.
By default, only a single build of a project is executed at a time — any other requests to start building that project will remain in the build queue until the first build is complete.
This is a safe default, as projects can often require exclusive access to certain resources, such as a database, or a piece of hardware.

But with this option enabled, if there are enough build executors available that can handle this project, then multiple builds of this project will take place in parallel. If there are not enough available executors at any point, any further build requests will be held in the build queue as normal.

Enabling concurrent builds is useful for projects that execute lengthy test suites, as it allows each build to contain a smaller number of changes, while the total turnaround time decreases as subsequent builds do not need to wait for previous test runs to complete.
This feature is also useful for parameterized projects, whose individual build executions — depending on the parameters used — can be completely independent from one another.


I want to build the project using  Execute shell::
====================================================
at Build step select the Execute shell

![image](https://github.com/user-attachments/assets/8038641b-162e-4b15-8790-7376d73b9324)



> git clone https://github.com/parasa7358/spring-petclinic.git

> cd spring-petclinic

> mvn install


06/03/2025::
==============

Pipelines Introduction:::

A Jenkins pipeline is a series of automated steps or stages that define the process of continuous integration/continuous delivery (CI/CD) for your code. Jenkins, being a popular open-source automation server, uses pipelines to automate tasks like building, testing, and deploying code.

There are two types of Jenkins pipelines:

1. Declarative Pipeline
2. Scripted Pipeline

1. Declarative Pipeline::
The declarative pipeline syntax is simpler and more structured. It's the recommended style for most users because it's easy to read and maintain

Here's an example of a simple declarative pipeline:

pipeline{

agent any

stages{

Stage ('Clone'){

steps{

// write code
}
}

Stage ('Build'){
steps{

// write code
}
// write code

}

Stage ('Test'){

steps{

// write code
}
// write code

}
Stage ('Execute test casea and get the results'){

steps{

// write code
}
// write code

}

Stage ('Generated Artifact'){

steps{

// write code
}
// write code

}

Stage ('Deploy'){

steps{

// write code
}
// write code

}

// write code

}

}

Please try to create one pipeline job in jenkinsfile and execute the below Declarative pipeline example:;


pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'feature/2025.02.27', url: 'git@github.com:parasa7358/spring-petclinic.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Test Results Reports') {
            steps {
                junit 'target/surefire-reports/*.xml'
            }
        }
        
        stage('Artifacts') {
            steps {
                archiveArtifacts artifacts: 'target/*.war', followSymlinks: false
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello World'
            }
        }
    }
}



Key elements in the declarative pipeline:::
======================================
pipeline: This is the top-level structure.
agent: Specifies where the pipeline will run, such as on any available agent, a specific node, or a Docker container.
stages: Defines the different steps or stages in the pipeline (e.g., Build, Test, Deploy).
steps: Commands to be executed in each stage.


2. Scripted Pipeline::
   ==============

The scripted pipeline offers more flexibility, but it is less structured and can be harder to maintain. It uses Groovy syntax to define the pipeline.

Here's an example of a scripted pipeline:

node {
    try {
        stage('Build') {
            echo 'Building the application...'
            // Your build commands here
        }
        
        stage('Test') {
            echo 'Running tests...'
            // Your test commands here
        }

        stage('Deploy') {
            echo 'Deploying the application...'
            // Your deploy commands here
        }


        Please try to create one new jenkins pipeline job and execute below script for Scripted pipeline examples

        node {
        stage('Clone') {
                git branch: 'master', url: 'https://github.com/parasa7358/onlinebookstore.git'
			}
			
			 stage('Build') {
        
                sh 'mvn package'
        
			}
			stage('Test') {
        
                sh 'mvn test'
        
			}
        }



  Key differences in a scripted pipeline:::
  ==================================
node: Represents a Jenkins agent where the pipeline will run.


07/03/2025::
===============

Pipeline as Code::
==================
Both declarative and scripted pipelines are stored as Jenkinsfiles, which you place in your source code repository. This allows you to version control your pipeline and keep it aligned with your application code.

Declarative pipeline with Jenkinsfile::
===============================

pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'git@github.com:parasa7358/spring-petclinic.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Test Results Reports') {
            steps {
                junit 'target/surefire-reports/*.xml'
            }
        }
        
        stage('Artifacts') {
            steps {
                archiveArtifacts artifacts: 'target/*.war', followSymlinks: false
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello World'
            }
        }
    }
}


This pipeline:::

1 Checks out the source code from your Git repository.
2. Builds the project using Maven.
3.Runs unit tests.
4.Deploys the application using a custom script.

JOb creation::

![image](https://github.com/user-attachments/assets/dacaf03a-5557-44ce-88ba-0b230ed061cb)

Branches to build

![image](https://github.com/user-attachments/assets/64065ba7-534e-4771-a667-00d5f64e5a4b)

Script Path::: This path is Jenkinsfiles where we maintained in github source code level

![image](https://github.com/user-attachments/assets/3b4783f0-c613-45d1-81a7-00712a79f5ad)


Scripted pipeline with Jenkinsfile::
===============================

node {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'git@github.com:parasa7358/spring-petclinic.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Test Results Reports') {
            steps {
                junit 'target/surefire-reports/*.xml'
            }
        }
        
        stage('Artifacts') {
            steps {
                archiveArtifacts artifacts: 'target/*.war', followSymlinks: false
            }
        }
        stage('Deploy') {
            steps {
                echo 'Hello World'
            }
        }
    }
}

github sourcecode jenkinsfile 

![image](https://github.com/user-attachments/assets/44f93ca7-1d95-4efb-afad-cc262de61dbe)


Create AWS Free tier Account::
================================


Please go throw the recorded video session and follow the steps to create the free tier AWS account


10/03/2025::
==============

Tomcat Web Server: Introduction
===============

Apache Tomcat is an open-source web server and servlet container developed by the Apache Software Foundation. It is primarily used to serve Java applications and is one of the most popular servlet containers in the world.

Tomcat is an essential tool for anyone working with Java web applications. It provides a simple, reliable platform for deploying and managing Java Servlets and JSPs and is widely used in both development and production environments. Its ease of use, combined with powerful features and flexibility, makes it an ideal choice for many developers working on Java-based web applications.

Apache Tomcat is an open-source web server and servlet container that is primarily used to serve Java-based web applications. It implements several Java EE (Enterprise Edition) specifications, such as Java Servlet, JavaServer Pages (JSP), and WebSocket, among others. Tomcat is often used to run Java applications on the web because it's lightweight, easy to configure, and widely supported.

Here are some key points about Tomcat:

1. **Servlet Container**: Tomcat is a servlet container, meaning it manages the lifecycle of Java Servlets, which are small Java programs that run on a web server.
  
2. **JSP Support**: Tomcat also supports JavaServer Pages (JSP), a technology that allows for embedding Java code within HTML pages.

3. **Configuration**: It’s highly configurable through XML files, like `server.xml` for server settings, `web.xml` for application settings, and others.

4. **Lightweight**: Unlike full-fledged application servers like WildFly (formerly JBoss) or GlassFish, Tomcat is primarily a servlet and JSP container, which makes it lighter and easier to deploy for simpler Java web applications.

5. **Performance**: It’s known for good performance in handling static content, making it a popular choice for Java web developers.


Integrate Jenkins with Tomcat::
==============================



![image](https://github.com/user-attachments/assets/1d3919a7-585b-4737-9d60-95207ca08ad8)


![image](https://github.com/user-attachments/assets/0d1d5e30-6da8-485a-937f-b04c50e15351)



Integrating Tomcat with Jenkins is a common use case for automating the deployment of Java-based web applications. Jenkins can be set up to deploy a web application to a Tomcat server whenever a new build is triggered.

Prerequisites:

Apache Tomcat should be installed and running on your server.
Jenkins should be installed and running.

Steps to integrate Jenkins with Tomcat:

1. Install the "Deploy to Container" Plugin in Jenkins:
The easiest way to deploy to Tomcat from Jenkins is by using the Deploy to Container plugin. This plugin allows Jenkins to deploy WAR files to a Tomcat server.

Go to your Jenkins dashboard.
Click on Manage Jenkins > Manage Plugins.
In the Available tab, search for Deploy to Container Plugin and install it.
Once installed, restart Jenkins to apply the plugin.

2. Configure Tomcat Server in Jenkins:
Now you need to tell Jenkins where your Tomcat server is running.

In Jenkins, go to Manage Jenkins > Configure System.
Scroll down to the Deploy to container section.
Click Add Tomcat Server.

Provide the necessary information:
Name: Give the Tomcat server a name (Tomcat9).
URL: The URL of your Tomcat server (e.g., http://localhost:8080).
Username: The username for Tomcat's manager app (usually admin).
Password: The password for that username (set in Tomcat's tomcat-users.xml).
Save the configuration.

3. Configure Tomcat’s tomcat-users.xml:
Make sure Tomcat is set up to allow Jenkins to deploy the application by editing the tomcat-users.xml file.

https://stackoverflow.com/questions/7763560/401-unauthorized-error-while-logging-in-manager-app-of-tomcat

tomcat-users.xml file::
=========================

![image](https://github.com/user-attachments/assets/61a0b6ae-1e6c-47d0-8852-b226d65f38a4)



  <role rolename="manager-gui"/>
  <role rolename="manager-script"/>
  <role rolename="manager-jmx"/>
  <role rolename="manager-status"/>
  <role rolename="admin-gui"/>
  <role rolename="admin-script"/>
  <user username="admin" password="admin" roles="manager-gui, manager-script, manager-jmx, manager-status, admin-gui, admin-script"/>




Restart Tomcat to apply the changes.

4. Create a Jenkins Job to Build and Deploy the Application:
Next, you need to create a Jenkins job that will build your web application (e.g., a WAR file) and deploy it to Tomcat.

From the Jenkins dashboard, click New Item.

Select Freestyle Project, give it a name, and click OK.

In the job configuration, go to the Build section and configure your build step, such as building a Maven project For Maven, you can use:

> mvn clean install

In the Post-build Actions section, add Deploy war/ear to a container.

In the WAR/EAR files field, provide the path to your WAR file (e.g., target/my-app.war).
In the Container field, choose the Tomcat server you configured earlier.
Set the Context Path (e.g., IfocusAWSDevOpsTraining), which is the URL path where the application will be accessible on Tomcat.
If you want Jenkins to deploy automatically after every successful build, check the option Deploy after every successful build.
Save the job.

5. Trigger the Build and Deployment:
Go to the Jenkins job you just created and click Build Now to trigger a build.
After the build completes, Jenkins should deploy the WAR file to your Tomcat server.

You can access your application by going to http://<tomcat_host>:<tomcat_port>/<context_path>

example::  http://localhost:8080/IfocusApplication/

POLL SCM:: * * * * * (every minute automatic build & deployment happend when new commits happend in github)
This setup will allow Jenkins to automatically build and deploy your Java web application to Tomcat with each new build



11/03/2025::
=================

Deploy Onlinebookstore/spring-petclinic applications to target server (Tomcat)::
=====================================================================================================================

please create one new pipeline job

Provide the Description

![image](https://github.com/user-attachments/assets/458b8076-ebce-4ac0-932e-64ee5a6e460b)

Enabled POLL SCM

![image](https://github.com/user-attachments/assets/5b5ae6d9-987a-4c54-9450-c3a89497be29)

In Pipeline Section write groovy script using Declarative style 


![image](https://github.com/user-attachments/assets/5d624b7b-9224-4d20-863f-0f3e4671916e)

Script::
=======

pipeline
{
    agent any

    tools{

        maven 'maven'
    }

stages{
stage('Git checkout'){

    steps{

        git branch: 'main' url: 'https://github.com/parasa7358/Petclinic.git'

    }
}

stage('clean and install'){

    steps{

      sh 'mvn clean install'

    }
}

stage('Package'){

    steps{

      sh 'mvn package'

    }
}

stage('Archive the Artifacts'){

    steps{

      sh 'mvn clean install'
    }
    post{
        success{

            archiveArtifacts artifacts: '**target/*.war'
        }
    }

    }


stage('Test Cases'){

    steps{

      sh 'mvn test'

    }
}


stage('Deploy to tomcat server'){

    steps{

      deploy adapters: [tomcat9(credentialsId: 'tomcat9credentials', path: '', url: 'http://localhost:8080/')], contextPath: 'Ifocus Solutions Pvt Ltd', war: '**/*.war'

    }
}

}
}


Run the job


![image](https://github.com/user-attachments/assets/f240a720-41dd-4bc0-955d-a247b1cf8918)

![image](https://github.com/user-attachments/assets/369955cf-0f1c-4ae1-bae3-3870edc0e282)


12/03/2025::
=================

Integrate Jenkins with Tomcat using Declarative Approach::
============================================

To integrate Jenkins with Tomcat using the Declarative Pipeline approach, you'll be using Jenkins Pipeline syntax to automate the deployment process to a Tomcat server. This process typically involves building the application, packaging it, and then deploying it to Tomcat.

1. Jenkinsfile Configuration (Declarative Pipeline)

In your Jenkins project, you'll create a Jenkinsfile, which contains the Declarative Pipeline syntax. This file defines the steps involved in the CI/CD pipeline.

Please execute below script in jenkins pipeline job using Declarative style

pipeline
{
    agent any

    tools{

        maven 'maven'
    }

stages{
stage('Git checkout'){

    steps{

        git branch: 'feature/2025.03.12', url: 'https://github.com/parasa7358/Petclinic.git'

    }
}

stage('clean and install'){

    steps{

      sh 'mvn clean install'

    }
}

stage('Package'){

    steps{

      sh 'mvn package'

    }
}

stage('Archive the Artifacts'){

    steps{

      sh 'mvn clean install'
    }
    post{
        success{

            archiveArtifacts artifacts: '**target/*.war'
        }
    }

    }


stage('Test Cases'){

    steps{

      sh 'mvn test'

    }
}


stage('Deploy to tomcat server'){

    steps{

      deploy adapters: [tomcat9(credentialsId: 'tomcat9credentials', path: '', url: 'http://localhost:8080/')], contextPath: 'Ifocus Solutions Pvt Ltd', war: '**/*.war'

    }
}

}
}

13/03/2025::
=================

To integrate SonarQube with Jenkins, you need to ensure that Jenkins can communicate with your SonarQube server to perform static code analysis during your CI/CD pipeline. This will allow you to analyze your code quality and get reports from SonarQube as part of your build process.

Here's how you can integrate SonarQube with Jenkins:please follow below steps

1. Install the SonarQube Plugin in Jenkins
Before you start, ensure that you have the SonarQube Scanner Plugin installed in Jenkins:

Go to Jenkins Dashboard.
Click on Manage Jenkins → Plugins.
Go to the Available tab, and search for SonarQube Scanner.
Install it and restart Jenkins.

2. Configure SonarQube in Jenkins
Next, you need to configure SonarQube on Jenkins so it can communicate with your SonarQube server.

Steps:
=====
Go to Jenkins Dashboard.
Click on Manage Jenkins → Configure System.
Scroll down to the SonarQube servers section and click Add SonarQube.

Fill in the following details:
=======================
Name::: Give your SonarQube instance a name (SonarQubeServer).
Server URL: URL to your SonarQube instance (e.g., http://localhost:9000). and default port is 9000
Server Authentication Token: You can generate a token in SonarQube by navigating to My Account → Security → Generate Tokens. Paste this token into Jenkins.
Click Save.

3. Configure the SonarQube Scanner in JenkinsSteps:
 ===============================================
In the Configure System page, scroll to the SonarQube Scanner section.
Click Add SonarQube Scanner and select SonarQube Scanner for Jenkins.

If you want to use a custom installation, specify the path to the SonarQube Scanner binary.
Click Save.

 Configure SonarQube Project::
 ========================
Go to your SonarQube server (e.g., http://localhost:9000).
Create a project or use an existing one.
Obtain the Project Key from the SonarQube project and update the pipeline script as shown in the sonar.projectKey parameter.

Go to Projects and click Local project

![image](https://github.com/user-attachments/assets/0b177021-0fc2-4ba4-a987-fee4a3420717)

Click Next

![image](https://github.com/user-attachments/assets/2cccbec2-463b-47ab-9379-f02244272f3a)

Selected Use the global setting

![image](https://github.com/user-attachments/assets/702766f0-01a9-4919-bbda-acb3a8996dcd)

Click Create Project

![image](https://github.com/user-attachments/assets/a614a64f-7171-43c3-b19e-787e13ee0c16)

Now Spring-petclinic Project created in Sonarqube

![image](https://github.com/user-attachments/assets/0f79347c-8bde-4fa3-8eaa-3ca91a27422d)

Click Locally

![image](https://github.com/user-attachments/assets/d6e4fa35-299c-4768-b291-c669d9b52995)

![image](https://github.com/user-attachments/assets/ba49dbeb-8f7f-4fb4-ab7d-8c4d3644a133)

Click Generate for Token

Analyze "spring-petclinic12": sqp_0eb364758c5186bea4077eff841ddb99ba89a3ab


![image](https://github.com/user-attachments/assets/7e46dded-06da-467a-8838-62e9f0337a7a)

Click Continue

![image](https://github.com/user-attachments/assets/590c723c-0df3-48df-bf7d-77575e63614a)

![image](https://github.com/user-attachments/assets/ace61156-d25b-4d00-b248-d5bd0b1de835)

Selected Maven and copy below script from sonarqube and it will help to integrate Sonarqube with jenkins pipeline

![image](https://github.com/user-attachments/assets/1da2fbb2-5118-45e5-85ec-c7767a44529b)


mvn clean verify sonar:sonar \
  -Dsonar.projectKey=spring-petclinic12 \
  -Dsonar.projectName='spring-petclinic12' \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.token=sqp_0eb364758c5186bea4077eff841ddb99ba89a3ab


  IntegrateSonarqubeWithJenkins::
  ==================================

  Go To jenkins and create new job IntegrateSonarqubeWithJenkins

  ![image](https://github.com/user-attachments/assets/dc7d3f1e-5852-4288-bf00-5537b6a4935c)

Please use below script to run the pipeline job

pipeline
{
    agent any

    tools{

        maven 'maven'
    }

stages{
stage('Git checkout'){

    steps{

        git branch: 'main', url: 'https://github.com/parasa7358/Petclinic.git'

    }
}

stage('clean and install'){

    steps{

      sh 'mvn clean install'

    }
}

stage('Package'){

    steps{

      sh 'mvn package'

    }
}

stage('Archive the Artifacts'){

    steps{

      sh 'mvn clean install'
    }
    post{
        success{

            archiveArtifacts artifacts: '**target/*.war'
        }
    }

    }


stage('Test Cases'){

    steps{

      sh 'mvn test'

    }
}

stage('Sonarqube Analysis'){

    steps{

      sh 'mvn clean package'

    sh '''mvn sonar:sonar \
  -Dsonar.projectKey='spring-petclinic' \
  -Dsonar.projectName='spring-petclinic' \
  -Dsonar.host.url='http://localhost:9000' \
  -Dsonar.token=sqp_8d74d659dbf3d3bf2924a0d24104f5ddba914fac'''

    }
}


stage('Deploy to tomcat server'){

    steps{

      deploy adapters: [tomcat9(credentialsId: 'tomcat9credentials', path: '', url: 'http://localhost:8080/')], contextPath: 'Ifocus Solutions Pvt Ltd', war: '**/*.war'

    }
}

}
}

After completed the CI/CD

![image](https://github.com/user-attachments/assets/80d28918-53d6-4c3a-881a-5b064030a04c)

![image](https://github.com/user-attachments/assets/9da10f2f-6114-4fbb-ac59-d052298c576c)

![image](https://github.com/user-attachments/assets/fd461a17-e1f9-473c-aaca-2073c0e193c6)


7. Running the Pipeline
Once the pipeline is configured, Jenkins will execute the SonarQube analysis during the build process. After the build completes, you can view the analysis results in your SonarQube dashboard.

8. View SonarQube Reports
After the analysis is complete, you can view detailed reports about code quality, such as:

https://dzone.com/articles/getting-tsql-project-scanned-with-sonarqube

![image](https://github.com/user-attachments/assets/ea965310-c76b-4ea1-9a12-de51d2573668)

![image](https://github.com/user-attachments/assets/2b006ce0-f207-4655-ac8f-08925271580d)

![image](https://github.com/user-attachments/assets/7a0f8a82-5843-44e1-b7b5-b5e4a387db9c)



Code coverage
Code smells
Bugs
Vulnerabilities
Duplications
These reports will be available in the SonarQube dashboard for your project.


14/03/2025::
================

Jfrog Artifactory Overview::
======================

JFrog Artifactory is a universal artifact repository manager that serves as a central hub for storing, managing, and distributing software artifacts, binaries, packages, and other assets throughout the software development lifecycle, improving automation, and ensuring release integrity.

Artifact Repository Management:

Allows for storing binaries and artifacts (e.g., libraries, packages, Docker images) in a centralized location.
Supports all major package types (e.g., Maven, Gradle, npm, NuGet, RubyGems, etc.).
Version Control:

Helps in managing versions of your artifacts and ensures the correct version is used during builds and deployments.
Integration with CI/CD:

Integrates seamlessly with CI/CD tools like Jenkins, Bamboo, GitLab CI, and others.
Enables automated publishing of artifacts as part of your continuous integration pipeline.
Access Control & Security:

Provides fine-grained access control and permissions for users and groups.
Supports user authentication, security, and audit trails to ensure compliance and secure artifact management.
Replication:

Allows you to replicate artifacts across multiple Artifactory instances, ensuring high availability and disaster recovery capabilities.
Remote Repositories:

Artifactory can proxy remote repositories, allowing you to cache and fetch external dependencies without re-downloading them each time.
Promotion & Release Management:

You can "promote" artifacts from one repository to another (e.g., from a development repository to a production repository), allowing for better control over releases.
Multi-Platform Support:

Artifactory supports multiple programming languages and platforms, making it a universal solution for managing software dependencies and releases.

17/03/2025::
=================

Integarte Jfrog with Jenkins::
===========================

<img width="846" alt="Jfrog" src="https://github.com/user-attachments/assets/5d07c387-99b9-43e0-97c6-b3b8e008da31" />

First Step:: 
https://jfrog.com/download-jfrog-platform/  ---download url

![image](https://github.com/user-attachments/assets/6ef7f0ee-d89e-4c84-8764-17bcde0c18b3)

previous versions link

https://jfrog.com/download-legacy/?product=artifactory&version=7.104.12

All zip version and search 6.12.1 OSS version

https://releases.jfrog.io/artifactory/bintray-artifactory/


Jfrog Script::
===============

stage ('Artifactory Server'){
            steps {
               rtServer (
                 id: "Artifactory",
                 url: 'http://localhost:8081/artifactory',
                 username: 'admin',
                  password: 'password',
                  bypassProxy: true,
                   timeout: 300
                        )
            }
        }
        stage('Upload'){
            steps{
                rtUpload (
                 serverId:"Artifactory" ,
                  spec: '''{
                   "files": [
                      {
                      "pattern": "*.war",
                      "target": "ifocus-solutions-pvt-ltd"
                      }
                            ]
                           }''',
                        )
            }
        }
        stage ('Publish build info') {
            steps {
                rtPublishBuildInfo (
                    serverId: "Artifactory"
                )
            }
        }

 installed plugin for artifactory (Jfrog)::
 =====================================


![image](https://github.com/user-attachments/assets/542a6be0-9059-4935-9658-81ce27634337)

After installed Artifactory plugin 

Go to Manage Jenkins--System configuration find JFROG

 ![image](https://github.com/user-attachments/assets/5ddbd986-aaee-478b-8a03-e117f53a7b3a)

Click JFrog Platform Instances

![image](https://github.com/user-attachments/assets/c176ad14-5982-4ea3-b960-468d00f851c7)

For user name and password
Go to Jfrogadmin-Securityusers
Default Jfrog U/P----admin/password

![image](https://github.com/user-attachments/assets/83204f3d-bf7b-4bd5-b616-61eaf03ae216)

![image](https://github.com/user-attachments/assets/2af4f08d-5778-4517-8b90-43037eb6ecce)

![image](https://github.com/user-attachments/assets/c104f1c1-6cd0-4911-8eef-b9243a2dd41f)


I need to setup target in Jfrog

ifocus-solutions-pvt-ltd

click Local repository

![image](https://github.com/user-attachments/assets/accda4b3-8ff1-412b-9dfb-c790ff8d9757)


Select maven

![image](https://github.com/user-attachments/assets/a711233f-8298-4fb9-84f7-3acd19d4e73c)

Repository key  :::: ifocus-solutions-pvt-ltd

![image](https://github.com/user-attachments/assets/97c49959-7963-475d-8efb-693952d973ea)

Click save and finish

![image](https://github.com/user-attachments/assets/a17b2e49-1e1a-408a-ad16-64cb6bd734b4)

Go to artifacts and check repository is created with name -ifocus-solutions-pvt-ltd

![image](https://github.com/user-attachments/assets/af618d7f-ba98-4b2f-8bd2-86fb7928bdae)

CI/CD all tools ans stages script:: create new job in jenkins and execute below script 
=====================================


pipeline
{
    agent any

    tools{

        maven 'maven'
    }

stages{
stage('Git checkout'){

    steps{

        git branch: 'main', url: 'https://github.com/parasa7358/Petclinic.git'

    }
}

stage('clean and install'){

    steps{

      sh 'mvn clean install'

    }
}

stage('Package'){

    steps{

      sh 'mvn package'

    }
}

stage('Archive the Artifacts'){

    steps{

      sh 'mvn clean install'
    }
    post{
        success{

            archiveArtifacts artifacts: '**target/*.war'
        }
    }

    }


stage('Test Cases'){

    steps{

      sh 'mvn test'

    }
}

stage('Sonarqube Analysis'){

    steps{

      sh 'mvn clean package'

    sh '''mvn sonar:sonar \
  -Dsonar.projectKey='spring-petclinic' \
  -Dsonar.projectName='spring-petclinic' \
  -Dsonar.host.url='http://localhost:9000' \
  -Dsonar.token=sqp_8d74d659dbf3d3bf2924a0d24104f5ddba914fac'''

    }
}
stage ('Artifactory Server'){
            steps {
               rtServer (
                 id: "Artifactory",
                 url: 'http://localhost:8081/artifactory',
                 username: 'admin',
                  password: 'password',
                  bypassProxy: true,
                   timeout: 300
                        )
            }
        }
        stage('Upload'){
            steps{
                rtUpload (
                 serverId:"Artifactory" ,
                  spec: '''{
                   "files": [
                      {
                      "pattern": "*.war",
                      "target": "ifocus-solutions-pvt-ltd"
                      }
                            ]
                           }''',
                        )
            }
        }
        stage ('Publish build info') {
            steps {
                rtPublishBuildInfo (
                    serverId: "Artifactory"
                )
            }
        }

stage('Deploy to tomcat server'){

    steps{

      deploy adapters: [tomcat9(credentialsId: 'tomcat9credentials', path: '', url: 'http://localhost:8080/')], contextPath: 'Ifocus Solutions Pvt Ltd', war: '**/*.war'

    }
}

}
}



18/03/2025::
===============

AWS (Amazon Web Services)::
====================

Amazon Web Services (AWS) is a comprehensive and widely adopted cloud platform offered by Amazon. It provides a broad set of services to help organizations and individuals build and scale applications, manage data, and process workloads in the cloud. AWS is designed to provide flexible, scalable, and cost-effective solutions for computing, storage, networking, machine learning, and much more.

AWS ---Amazon web services

compute services::
Amazon EC2 (Elastic Compute Cloud): Provides scalable virtual servers to run applications.
AWS Lambda: Lets you run code without provisioning or managing servers. It automatically scales based on usage.

Storage services::
Amazon S3 (Simple Storage Service): Object storage for storing and retrieving large amounts of data.
Amazon EBS (Elastic Block Store): Persistent block-level storage for EC2 instances.

Database::
Amazon RDS (Relational Database Service): Managed relational database service supporting multiple database engines (e.g., MySQL, PostgreSQL, MariaDB, etc.).
Amazon DynamoDB: A managed NoSQL database service.
Amazon Aurora: A high-performance relational database engine compatible with MySQL and PostgreSQL.

Network services::
Amazon VPC (Virtual Private Cloud): Lets you create isolated networks within AWS for secure connections.

Security ::

AWS IAM (Identity and Access Management): Controls user access and permissions for AWS resources.
AWS KMS (Key Management Service): Managed service for creating and controlling encryption keys.
Security groups ---inbound, outbould roles


Containers & kuberneties::
ECS  ---elastic containers servcies
EKS  ----estastic kuberneties services
AKS  ---Azure kuberneties services

Cloud watch --Metrics Monitoring

CloudWatch Metrics allows you to track the performance and utilization of AWS resources such as EC2 instances, RDS databases, Lambda functions, S3 buckets, and much more.
These metrics include CPU utilization, disk activity, network traffic, and others. You can create custom metrics for your applications or services as well.

cloud trail ---Security Monitoring:

Use CloudTrail logs to detect unauthorized access or activity in your AWS environment. You can track changes in security settings, unauthorized API calls, or unexpected configuration changes.

Developer Tools::
AWS CodeCommit: Source control service for managing your code repositories.
AWS CodeDeploy: Automates code deployments to EC2 instances and Lambda.
AWS CodePipeline: Continuous integration and continuous delivery (CI/CD) service for automating the release pipeline.

AWS EC2 ::
===========
Amazon Elastic Compute Cloud (Amazon EC2) is one of the core services provided by Amazon Web Services (AWS)

Wide Variety of Instance Types:

EC2 instances are grouped into families based on the type of workload they are optimized for. Some common instance families include:
General Purpose: e.g., t3, m5 instances (balanced CPU, memory, and networking).
Compute Optimized: e.g., c5 instances (great for high-performance computing tasks).
Memory Optimized: e.g., r5, x1e instances (designed for high-memory workloads like databases).

create EC2 Ubuntu Linux Machine in AWS::
==================================

Go to AWS ans Search EC2

![image](https://github.com/user-attachments/assets/32cf433a-97b3-444f-9231-1c4aa1da6f79)

Click EC2

![image](https://github.com/user-attachments/assets/f54992d2-7d2b-4a1c-8395-ba5aee7d5899)

Go to instances at left side bar

![image](https://github.com/user-attachments/assets/fcaee5fc-c31a-40cd-a7da-0255afef4373)

Click Launch Instances, EC2  ---> Instances  -----> Launch an instance

![image](https://github.com/user-attachments/assets/9b6128c5-cf0e-48ee-bc11-93852cc3e166)

Select Ubuntu

![image](https://github.com/user-attachments/assets/f610aae5-e7a9-43f6-af7e-e16b6ce9becb)

Select Amazon Machine Image (AMI)

![image](https://github.com/user-attachments/assets/2e5e91a6-cd80-445b-9932-b9d760475be7)


select Instance type,t2 medium

![image](https://github.com/user-attachments/assets/47d6a619-cbe2-41d4-b2ca-40ae44988efb)


Create Create new key pair and provide key pair name

![image](https://github.com/user-attachments/assets/1526a72d-ba98-45be-8998-2d67788c73ef)

click create pair

![image](https://github.com/user-attachments/assets/66a6f77c-36b3-49d3-87a5-abe0358a3c3b)

click launch instance

![image](https://github.com/user-attachments/assets/dca82f59-824d-4cf2-9bf2-ffe81948993c)

instance will be created

![image](https://github.com/user-attachments/assets/ed110a9c-d118-4a08-b678-a3cf945ef5c7)



![image](https://github.com/user-attachments/assets/38ccd3b2-71ce-4102-a047-db937ab13080)



19/03/2025:::
=====================

Master & Node communication Via SSH keys::
================================

i have to create 2 EC2 ubuntu machines in AWS
1. Jenkinsmaster
2. Node

![image](https://github.com/user-attachments/assets/9fb55c6b-b0b5-4308-8061-91a23184b6db)


we have already .pem file dowloaded in you local machin

right click from .pem and click Open git bash here option
Now Go to AWS Ubuntu machine which is already created in AWS insatnces and select master machine

![image](https://github.com/user-attachments/assets/ae110666-3e1d-4a48-bfb4-ecb3790187f8)

Click Connect

![image](https://github.com/user-attachments/assets/4130c330-b01d-4a7c-b820-7b836db556b9)

Click SSH Client

![image](https://github.com/user-attachments/assets/fb0dfc0d-abbe-427c-a79b-a10df2f2410c)

Copy URL

>ssh -i "Newkeysmasternode.pem" ubuntu@ec2-18-237-178-192.us-west-2.compute.amazonaws.com

![image](https://github.com/user-attachments/assets/a0bf53d1-3b1a-42a0-8c40-8cb39f85cd09)

Now past that url in Gitbash

![image](https://github.com/user-attachments/assets/e52355e5-73b3-4d7b-9e04-3ce8cd72ffe5)

switch to root user below command run
>Sudo -i

![image](https://github.com/user-attachments/assets/98086ebc-bbd6-4757-ac12-923a2a6eb896)

update the all packages ,please run below command

>sudo apt-get update

![image](https://github.com/user-attachments/assets/3b291e76-4a2a-4d5a-bbd2-58231282e4b7)

Install JDK & Maven:;
============

JDK link

https://bluevps.com/blog/how-to-install-java-on-ubuntu

MAven link

https://phoenixnap.com/kb/install-maven-on-ubuntu



>sudo apt-get install maven
>java -version
>mvn -v

Set java home environment 

>sudo vi /etc/environment
JAVA_HOME=”/usr/lib/jvm/java-8-openjdk-amd64/jre”
MAVEN_HOME=”/usr/share/maven”

Reload your system environment
>source /etc/environment

Veriy the variables was set correctly
>echo $JAVA_HOME
>echo $MAVEN_HOME

Insatll Jenkins on master machine

https://phoenixnap.com/kb/install-jenkins-ubuntu


AWS any machines default password authentication is disabled , 
we need to enabled in any linux machines
>sudo vi /etc/ssh/sshd_config
>sudo service sshd restart
In EC2 – by default password based authentication is disabled so we need to enabled
>vi /etc/ssh/sshd_config
passwordauthentication :yes

![image](https://github.com/user-attachments/assets/99decb00-3ef0-4528-8e58-0d69bf14ce36)

In ubuntu machine default user is not sudo user,
>visudo
Jenkins ALL=(ALL:ALL) NOPASSWD:ALL
>su Jenkins
Switching to new user

![image](https://github.com/user-attachments/assets/86bc74b0-e31f-44aa-bcab-875ed9a3a016)

![image](https://github.com/user-attachments/assets/98b96a48-2ee3-466c-b917-26c1919b15f6)

Once installed Jenkins successfully
>we need to enabled the Inbounds and outbounds rules in AWS security groups

Inbounds rules

![image](https://github.com/user-attachments/assets/b7075d75-dd60-42d4-a282-7be861252685)

Copy public IP address and go to browser
Access Jenkins using Public IP address
http://35.86.160.156:8080/

bydefault Jenkins runs on port 8080
Jenkins home path/var/lib/Jenkins
How to change the port number in Jenkins::
https://stackoverflow.com/questions/28340877/how-to-change-port-number-for-jenkins-installation-in-ubuntu-12-04
>sudo nano /etc/default/jenkins


Now Go to Node Machine::
==============
Please insatll JDK & Maven in node machine and setup environemnt varibles

>sudo apt-get install maven
>java -version
>mvn -v
Set java home environment 

>sudo vi /etc/environment
JAVA_HOME=”/usr/lib/jvm/java-8-openjdk-amd64/jre”
MAVEN_HOME=”/usr/share/maven”

Reload your system environment
>source /etc/environment

Veriy the variables was set correctly
>echo $JAVA_HOME
>echo $MAVEN_HOME

comminicate master & node via SSH keys
>ssh-keygen
after generated copy public key to node machine

option-1 to copy keys from master to node
>ssh-copy-id user@ipaddressofnodemachine
>ssh-copy-id node@172.31.44.169

2nd option --copy keys manually from master to node

3rd options --i have created authorized_keys  file in node machine and copy public key from master to node

Master Node Configuration::
>got to manage Jenkins
>manage Nodes

>click new node
Remote root directory

![image](https://github.com/user-attachments/assets/774c7270-0607-4332-8679-ebad4a459979)

![image](https://github.com/user-attachments/assets/55da9a7b-3178-47cf-be6d-72b452a59b2d)

Launch methods via ssh

![image](https://github.com/user-attachments/assets/aa7e51ac-278f-473c-9512-bfb35422fea8)


Add credentials

![image](https://github.com/user-attachments/assets/2a3ae243-9a58-4666-bacd-317298d68f33)

>Host Key Verification Strategy
![image](https://github.com/user-attachments/assets/a926aed1-85d6-42e1-804f-da5df9792eed)


20/03/2025::
==============


Master Node Configuration::
>got to manage Jenkins
>manage Nodes
>click new node
Remote root directory

![image](https://github.com/user-attachments/assets/190f9e24-2842-4462-9773-6c98c7980d77)

![image](https://github.com/user-attachments/assets/10dcf0c4-7088-4071-a6e0-8f4729603029)
 
 

Launch methods via ssh

 ![image](https://github.com/user-attachments/assets/f25a3610-8d32-43ca-bde3-644426d37cb1)


Add credentials ::

option-1::

this time please use credentials option SSH key with private key from node machine

option::2 please use credentials with Username & password and let's try if you copy properly ,agent machine will conenct Successfully

 ![image](https://github.com/user-attachments/assets/d54e7393-a5b9-4194-8f50-c206b02c39d1)

 ![image](https://github.com/user-attachments/assets/2113f8d7-18d1-4e66-84ec-267c05fde9b5)

>Host Key Verification Strategy

 ![image](https://github.com/user-attachments/assets/58a7b48d-eab5-45a7-9661-1a72578ceda5)


Agent successfully connected

![image](https://github.com/user-attachments/assets/823523dc-fe3e-432c-b3d8-9c645483d30a)

 

Execute Jenkins job using slave 
Create one test slave job in Jenkins

>select Restrict where this project can be run

![image](https://github.com/user-attachments/assets/d6c206ac-06a1-4564-9351-7b35e4f4c521)


>select Label Expression

![image](https://github.com/user-attachments/assets/85b8897c-f6ec-4bd2-8bb9-3821251c20da)

please create 2 job in jenkins master and setup 1 job in Node machine and 2nd job master machine, just trigger Build Now 

Please observe below screenshot 2 job running different machines 

![image](https://github.com/user-attachments/assets/94005ac8-cb37-4c97-ba0e-14adf7c71566)

advantage of master & Node Integartion

![image](https://github.com/user-attachments/assets/5551bbab-46b7-49ae-b6c2-093299d2ecb2)

![image](https://github.com/user-attachments/assets/ac59dbc9-c012-44a0-ae98-0fbcc2d4e5d8)




21/03/2025::
=============

Ansible::
============

Ansible is an open-source automation tool used for configuration management, application deployment, task automation, and multi-node orchestration. It helps system administrators and DevOps professionals automate IT processes to improve efficiency, reduce errors, and simplify complex workflows.

![image](https://github.com/user-attachments/assets/c3d2b092-091c-479c-8198-e98dee9ab09f)


Key Features of Ansible:
================
Agentless: Ansible doesn't require any agents to be installed on the target machines. It uses SSH (or WinRM for Windows systems) to communicate with remote nodes.

Declarative Syntax: Ansible uses YAML (Yet Another Markup Language) to define the tasks, which makes it easy to read and write.

Idempotent: Ansible ensures that running the same playbook multiple times has the same effect, meaning it won’t reapply configurations if they’ve already been applied correctly.

Modular: Ansible has a large number of pre-built modules that can be used to manage various systems, applications, and services.

Playbooks: These are YAML files that describe the automation tasks you want to run. Playbooks are the heart of Ansible automation and define the "what" and "how" of your automation tasks.

Inventory Management: Ansible can manage an inventory of systems, which is used to organize and target different sets of machines.

Basic Components:
==================
Inventory: A list of hosts (machines) that Ansible will manage.

Playbook: A YAML file that defines the tasks and roles to be applied to the inventory.

Roles: A way to group related tasks and files together in a reusable manner.

Modules: Pre-built commands that Ansible can run on target systems to accomplish specific tasks (e.g., file management, system configuration, etc.).

3 linux ubuntu machines
AWS_Ubuntu 24
1)	AWS free tier 
a)ACS   ----Ansible control server

b)Node1
c)Node2


all these 3 machine ping to each other and see beow screenshots all 3 machines pings each other

![image](https://github.com/user-attachments/assets/08def171-c690-4c4c-8f93-17bdf9734c73)


Steps::
======
ubuntu@ip-172-31-28-207:~$ sudo -i
root@ip-172-31-28-207:~# su ansible
ansible@ip-172-31-28-207:/root$ cd ~
ansible@ip-172-31-28-207:~$ cd /etc/ansible/
ansible@ip-172-31-28-207:/etc/ansible$ ansible -m ping all
[WARNING]: Platform linux on host localhost is using the discovered Python interpreter at /usr/bin/python3.12, but future installation of
another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.17/reference_appendices/interpreter_discovery.html for more information.
localhost | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3.12"
    },
    "changed": false,
    "ping": "pong"
}
[WARNING]: Platform linux on host ansiblenode2@172.31.30.200 is using the discovered Python interpreter at /usr/bin/python3.12, but future
installation of another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.17/reference_appendices/interpreter_discovery.html for more information.
ansiblenode2@172.31.30.200 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3.12"
    },
    "changed": false,
    "ping": "pong"
}
[WARNING]: Platform linux on host ansiblenode1@172.31.20.135 is using the discovered Python interpreter at /usr/bin/python3.12, but future
installation of another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.17/reference_appendices/interpreter_discovery.html for more information.
ansiblenode1@172.31.20.135 | SUCCESS => {
    "ansible_facts": {
        "discovered_interpreter_python": "/usr/bin/python3.12"
    },
    "changed": false,
    "ping": "pong"
}
ansible@ip-172-31-28-207:/etc/ansible$



23/03/2025::
============

Ansible Playbooks Introduction::
==========================

Ansible playbooks are the heart of automation with Ansible. They are simple YAML (Yet Another Markup Language) files that define automation tasks in a structured, human-readable format. Playbooks allow you to automate configurations, deployments, and orchestration tasks in a clear and organized way.

Key Concepts::
==============

Playbook: A playbook is a file that contains one or more "plays." Each play defines a set of tasks to be executed on a group of hosts. The playbook can be used for things like installing packages, managing users, configuring services, etc.

Task: A task is an individual unit of work. Tasks define specific actions, such as installing a package, starting a service, or copying a file. Tasks are executed sequentially, in the order in which they are written in the playbook.

Inventory: An inventory is a list of hosts that Ansible will manage. The inventory file defines which machines to target. An inventory can group hosts together (e.g., web servers, db servers) for easy management.

Modules: Ansible provides numerous modules that are responsible for performing specific tasks like managing packages, services, files, etc. Common modules include apt, yum, service, copy, and file.


Structure of a Basic Playbook:
===============================
A basic playbook has the following components:

YAML Header: The file begins with a --- to indicate it’s a YAML file.

 the hosts (target machines)
 become: yes   ----->Sudo user 

Tasks: Tasks define the actions to be executed on the target systems.

![image](https://github.com/user-attachments/assets/71982463-6b41-4481-af94-29c76690b0b6)

I want to see where the Ansible is installed on ACS
>cd /etc/ansible

NOTE::
==========
Playbook is written in YAML format
Inside the playbook tasks
Each task is a module
Playbook is a one of yaml file
Yaml file is a collection of key-value pairsset of all tasks
Playbook is tell to the ansible what are the tasks can be performed
Each task  one module
Module is a smallest item of ansible
Module can be used to individual or smallest task can be performed
Any configuration management tool should maintain ‘state’


hosts: all (apply all we can be mentioned in inventory )
become: yes  (become user as a sudo user)
tasks:

we can search in google ansible playbook
https://docs.ansible.com/ansible/latest/user_guide/playbooks.html
https://docs.ansible.com/ansible/latest/user_guide/playbooks_intro.html#basics


install git example playbook::
==============================

---
- hosts: all

  become: yes
  
  tasks:
  
  -  name: install git
    
     apt:
     
       name: git
     
       state: present
     
       update_cache: yes

     
note:::default state is present 
update_cache: yes tells Ansible to run the apt-get update command on the remote machine before performing any further package operations (like installing or upgrading packages).
become: yes  # Elevate privileges to execute tasks as root

java install playbook::
https://www.geeksforgeeks.org/how-to-install-java-using-ansible-playbook/




java and git install playbook::
---
- hosts: all
  
  become: yes
  
  tasks:
  
  -  name: install git
    
     apt:
     
       name: git
     
       state: present
     
       update_cache: yes

  -  name: Install Java
    
     apt:
     
       name: openjdk-17-jdk
     
       state: present

>sudo vi demo.yml

copy git playbook code to demo.yml

---
- hosts: all
  
  become: yes
  
  tasks:
  
  -  name: install git
    
     apt:
     
       name: git
     
       state: present
     
       update_cache: yes

     

Run the playbook::
===============
>ansible-planbook <playbookname>
>ansible-playbook demo.yml

![image](https://github.com/user-attachments/assets/9bc02cd9-6749-4a09-a7d3-218110fd00d1)

ansible@ip-172-31-28-207:/etc/ansible$ ansible-playbook demo.yml

![image](https://github.com/user-attachments/assets/7df9edfc-af27-4815-b340-482237dfc368)


PLAY [all] **************************************************************************************************************************************

TASK [Gathering Facts] **************************************************************************************************************************
[WARNING]: Platform linux on host localhost is using the discovered Python interpreter at /usr/bin/python3.12, but future installation of
another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.17/reference_appendices/interpreter_discovery.html for more information.
ok: [localhost]
[WARNING]: Platform linux on host ansiblenode2@172.31.30.200 is using the discovered Python interpreter at /usr/bin/python3.12, but future
installation of another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.17/reference_appendices/interpreter_discovery.html for more information.
ok: [ansiblenode2@172.31.30.200]
[WARNING]: Platform linux on host ansiblenode1@172.31.20.135 is using the discovered Python interpreter at /usr/bin/python3.12, but future
installation of another Python interpreter could change the meaning of that path. See https://docs.ansible.com/ansible-
core/2.17/reference_appendices/interpreter_discovery.html for more information.
ok: [ansiblenode1@172.31.20.135]

TASK [install git] ******************************************************************************************************************************
ok: [localhost]
ok: [ansiblenode1@172.31.20.135]
ok: [ansiblenode2@172.31.30.200]

PLAY RECAP **************************************************************************************************************************************
ansiblenode1@172.31.20.135 : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
ansiblenode2@172.31.30.200 : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
localhost                  : ok=2    changed=0    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0

ansible@ip-172-31-28-207:/etc/ansible$


install git and jdk17 insatlled playbook::
======================================

---
- hosts: localhost
  
  become: yes
  
  tasks:
  
  -  name: install git
    
     apt:
     
       name: git
     
       state: present
     
       update_cache: yes
     
  -   name: Install Java jdk17 on ubuntu machine
 
      apt:
      
        name: openjdk-8-jdk
      
        state: absent
      
        update_cache: yes

Usefull Google links::
===========

https://docs.ansible.com/ansible/2.9/modules/list_of_all_modules.html
https://docs.ansible.com/ansible/2.9/modules/apt_module.html#parameters
https://www.geeksforgeeks.org/how-to-install-java-using-ansible-playbook/
https://www.yamllint.com/
https://www.geeksforgeeks.org/how-to-install-tomcat-using-ansible-playbook/






24/03/2025::
==============

Ansible all modules::
https://docs.ansible.com/ansible/latest/modules/list_of_all_modules.html
https://docs.ansible.com/ansible/2.9/modules/list_of_all_modules.html

Executing ansible in 2 ways
1.	Adhoc command  yearly base
2.	Playbook (YAML/YML) format use for repetitive work

When we can use adhoc commands  ->I want restart servers yearly base 

if you can use system inventory, below is the command
>ansible-playbook <playbookname>
>ansible-playbook hello-world.yml

I don’t want to use system level inventory

Inventory::
==========
where hosts/ipaddress are stored

I want to create my own inventory

>Cd /etc/ansible

![image](https://github.com/user-attachments/assets/e03cd989-34e8-46f5-88d0-9af56f11b6d9)

![image](https://github.com/user-attachments/assets/7a4d1993-1c1e-4da6-94b0-eeb105cb0d36)

![image](https://github.com/user-attachments/assets/79f8fb33-19d1-47a9-b26e-aff30d75d408)

>cat /etc/ansible/hosts

Sudo vi hosts

Copy all hosts

![image](https://github.com/user-attachments/assets/bcda07ba-ab66-4b86-bf67-f7ad9c556230)

I want categories into Inventory groups::
===================================

In Ansible, inventory groups are used to organize and categorize hosts (machines or servers) into logical groups. This allows you to apply tasks to specific sets of servers, simplifying playbook management and execution. An inventory is a list of managed hosts and their associated metadata, and groups are one of the key components of that structure.

Here’s a detailed explanation of Ansible inventory groups

1. What Are Inventory Groups?
An inventory group in Ansible is a way to group hosts based on a shared characteristic. For example, you might have groups for different environments (e.g., dev, prod), different types of servers (e.g., web_servers, db_servers), or other logical categories that fit your needs.

static inventory groups defined in the standard INI or YAML format.

# Define groups of hosts:: >sudo vi hosts

[web_servers]

 ansiblenode1@172.31.20.135
 
 ansiblenode2@172.31.30.200
 
 localhost
 
[db_servers]

ansiblenode1@172.31.20.135

ansiblenode2@172.31.30.200

[app_servers]

 localhost
 
i want to insatll 3 spfwares :: below playbook name -----> installsoftware.yml
==============================

---
- hosts: web_server
  
  become: yes
  
  tasks:
  
  -  name: install git
    
     apt:
     
       name: git
     
       state: present
     
       update_cache: yes

  -  name: install tree
    
     apt:
     
       name: tree
     
       state: present  

  -  name: install apache
  
     apt:
     
       name: apache2
     
       state: present

once above two files created run the below command

>ansible-playbook -i hosts installsoftware.yml
     
![image](https://github.com/user-attachments/assets/36d33a9a-b113-402c-80f7-1e9c404a245b)

>ansible -i hosts -m ping Webserver

Best practice is you need to create our own inventories

>sudo vi hosts

after ran the above yaml, please try to access all machines with IPaddresss

![image](https://github.com/user-attachments/assets/4a7778cd-6b97-4822-ad5e-11bbdde82231)

![image](https://github.com/user-attachments/assets/96a67d2a-993a-47ff-aa79-3dc8cd7aa06a)

![image](https://github.com/user-attachments/assets/01ee5e45-446e-42f2-a47f-c8b3e2fbe2f5)

Please enabled Inbound and Outbound rules::
=======================================

Inbound and outbound rules refer to the types of network traffic that are allowed or denied to and from a system, such as a server, virtual machine, or network device. These rules are typically defined in firewalls or security groups (such as in cloud environments like AWS, Azure, or Google Cloud). The primary goal is to control which data can enter or leave a network, ensuring security and proper access control.

Here’s a detailed explanation of inbound and outbound rules:

 Inbound Rules::
Inbound rules control traffic entering a system or network. These rules define which types of external traffic are allowed to reach a server, instance, or device.

Common Uses:
Allowing specific users or services to access the system.

Restricting access to the system from unauthorized users.

Opening ports for services like web servers (HTTP, HTTPS), SSH, database connections, etc

Allowing incoming traffic on port 80 (HTTP) so that users can access a web server.

Outbound Rules::
Outbound rules control traffic leaving a system or network. These rules define which traffic is allowed to exit a server or device and reach external destinations.

Common Uses:
Allowing a server to access external services like APIs, databases, or external servers.

Restricting unwanted traffic from the system to external destinations.

Controlling the flow of outgoing traffic to ensure compliance with security policies.

Allow HTTP/HTTPS: Allow outbound traffic on ports 80 (HTTP) and 443 (HTTPS) to any IP:



![image](https://github.com/user-attachments/assets/0e51f799-d746-45a5-94cb-f358ade65ba2)

![image](https://github.com/user-attachments/assets/8fa024b7-0999-40f7-94cb-3eaa018fbd41)

![image](https://github.com/user-attachments/assets/2ca3de47-8bea-4f5a-a35e-0238788cb7c7)



25/03/2025::
===================

Install LAMP on ubuntu 24.04::
==================================

A LAMP stack stands for Linux, Apache, MySQL, and PHP, which is a popular open-source software stack used for web development. It provides everything you need to set up a dynamic website or web application.

Here’s a quick overview of each component:

Linux: The operating system (in this case, Ubuntu).

Apache: The web server that serves your website’s files.

MySQL: The database management system for storing and retrieving data.

PHP: The programming language used for dynamic web page generation.



Manual Steps::
====================

https://www.digitalocean.com/community/tutorials/how-to-install-lamp-stack-on-ubuntu

>sudo apt update

>sudo apt install apache2

>sudo apt install mysql-server

>sudo apt install php

>sudo apt install libapache2-mod-php

>sudo apt install php-mysql

>sudo systemctl restart apache2

>sudo apt install php-cli

>sudo nano /var/www/html/info.php

above steps are manually installed all required softwares in LAMP project but my requirement is to write a Playbook for those manuall steps

Playbook for LAMP::  phppackage.yml
=====================



---
- hosts: all

  become: yes

  tasks:
  
  -  name: install apache2

     apt:

     name: apache2

     state: present

     update_cache: yes

  -  name: install php

      apt:

      name: php

      state: present  

  -  name: install mysql-server

     apt:

      name: mysql-server

      state: present
     
  -  name: install libapache2-mod-php

     apt:

     name: libapache2-mod-php

     state: present
                   
  -  name: install  php-mysql

     apt:

     name: php-mysql

     state: present
     
  -  name: restart apache

     service:

     name: apache2

      enabled: true

     state: restarted

  -  name: install php-cli

     apt:

     name: php-cli

      state: present 

  -  name: copy module info.php

     copy:

     src: info.php

     dest: /var/www/html/info.php     


Copy Module::
=========

https://docs.ansible.com/ansible/latest/collections/ansible/builtin/copy_module.html

Service Module::
==================

https://docs.ansible.com/ansible/latest/collections/ansible/builtin/service_module.html

info.php ::
==========


hosts grouping:
================

![image](https://github.com/user-attachments/assets/2eb4e4d2-bda2-44fa-8e86-d4b5bd51ed9e)


[Webservers]
ansiblenode1@172.31.20.135
ansiblenode2@172.31.30.200
localhost

[Appservers]
ansiblenode1@172.31.20.135

[DBservers]

localhost


Reference flow::
==============
ansible@ip-172-31-28-207:/etc/ansible/playbook$ ls
hosts  info.php  installsoftwares.yml  phppackage.yml
ansible@ip-172-31-28-207:/etc/ansible/playbook$ sudo vi phppackage.yml
ansible@ip-172-31-28-207:/etc/ansible/playbook$ sudo vi hosts
ansible@ip-172-31-28-207:/etc/ansible/playbook$ sudo vi phppackage.yml
ansible@ip-172-31-28-207:/etc/ansible/playbook$ ansible-playbook -i hosts phppackage.yml
ansible@ip-172-31-28-207:/etc/ansible/playbook$ sudo vi info.php
ansible@ip-172-31-28-207:/etc/ansible/playbook$ ansible-playbook -i hosts phppackage.yml

PLAY [Webservers] *********************************************************************************************

TASK [Gathering Facts] ****************************************************************************************
[WARNING]: Platform linux on host localhost is using the discovered Python interpreter at /usr/bin/python3.12,
but future installation of another Python interpreter could change the meaning of that path. See
https://docs.ansible.com/ansible-core/2.17/reference_appendices/interpreter_discovery.html for more
information.
ok: [localhost]
[WARNING]: Platform linux on host ansiblenode2@172.31.30.200 is using the discovered Python interpreter at
/usr/bin/python3.12, but future installation of another Python interpreter could change the meaning of that
path. See https://docs.ansible.com/ansible-core/2.17/reference_appendices/interpreter_discovery.html for more
information.
ok: [ansiblenode2@172.31.30.200]
[WARNING]: Platform linux on host ansiblenode1@172.31.20.135 is using the discovered Python interpreter at
/usr/bin/python3.12, but future installation of another Python interpreter could change the meaning of that
path. See https://docs.ansible.com/ansible-core/2.17/reference_appendices/interpreter_discovery.html for more
information.
ok: [ansiblenode1@172.31.20.135]

TASK [install apache2] ****************************************************************************************
ok: [ansiblenode2@172.31.30.200]
ok: [ansiblenode1@172.31.20.135]
ok: [localhost]

TASK [install php] ********************************************************************************************
ok: [ansiblenode1@172.31.20.135]
ok: [ansiblenode2@172.31.30.200]
ok: [localhost]

TASK [install mysql-server] ***********************************************************************************
ok: [ansiblenode1@172.31.20.135]
ok: [ansiblenode2@172.31.30.200]
ok: [localhost]

TASK [install libapache2-mod-php] *****************************************************************************
ok: [ansiblenode1@172.31.20.135]
ok: [ansiblenode2@172.31.30.200]
ok: [localhost]

TASK [install  php-mysql] *************************************************************************************
ok: [ansiblenode1@172.31.20.135]
ok: [ansiblenode2@172.31.30.200]
ok: [localhost]

TASK [restart apache] *****************************************************************************************
changed: [ansiblenode2@172.31.30.200]
changed: [localhost]
changed: [ansiblenode1@172.31.20.135]

TASK [install php-cli] ****************************************************************************************
ok: [ansiblenode1@172.31.20.135]
ok: [localhost]
ok: [ansiblenode2@172.31.30.200]

TASK [copy module info.php] ***********************************************************************************
changed: [localhost]
changed: [ansiblenode2@172.31.30.200]
changed: [ansiblenode1@172.31.20.135]

PLAY RECAP ****************************************************************************************************
ansiblenode1@172.31.20.135 : ok=9    changed=2    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
ansiblenode2@172.31.30.200 : ok=9    changed=2    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0
localhost                  : ok=9    changed=2    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0



Please execute above steps we will see the php insatlled on all 3 machines

![image](https://github.com/user-attachments/assets/d49aa2d0-69ad-4c40-8408-2ccf3edbf838)

![image](https://github.com/user-attachments/assets/74b9e6dd-8fb1-452f-85f1-faffd48d7dae)

![image](https://github.com/user-attachments/assets/6d58255a-e6ea-44b7-a4e2-39f8598358b3)


info.php::
===========

<html>
  <head>
    <title>your_domain website</title>
  </head>
  <body>
    <h1>Hello World!</h1>

    <p>This is the landing page of <strong>your_domain</strong>.</p>
  </body>
  <body>
    <h1>Hello World!</h1>

    <p>This is the landing page of <strong>your_domain</strong>.</p>
  </body>
</html>





26/03/2025::
===============

loop::

In Ansible, loops are used to repeat tasks over a list of items, making automation more efficient and reducing redundancy in playbooks. You can loop through arrays, dictionaries, and other types of data in Ansible to execute tasks multiple times.

There are several ways to use loops in Ansible, and here are the most common methods:

1. Using loop keyword
The loop keyword is the most common way to iterate over a list of items. Here's an example of how to use it:

https://spacelift.io/blog/ansible-loops

https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_loops.html

https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_loops.html


Examples::
==========

---
- hosts: Webservers

  become: yes

  tasks:

    - name: Install all packages
   
      apt:
    
	name: "{{ item }}"

        state: latest

     loop:
        -  apache2
        -  php
        -  php-mysql
        -  libapache2-mod-php
        -  php-cli
    -  name: restart apache

        service:

       name: apache2

        enabled: true

       state: restarted

    -  name: copy module info.php

       copy:

       src: info.php

       dest: /var/www/html/info.php  



Setup module in ansible::
============================


https://docs.ansible.com/ansible/latest/collections/ansible/builtin/setup_module.html
Setup module is used to collect the facts
Facts information gather from nodes called facts
>ansible -I hosts -m setup Webserver

Using filter command

>ansible -i hosts -m setup -a "filter=*os*" Webserver

ansible_os_family": "Debian"

Ansible when statements

https://docs.ansible.com/ansible/latest/user_guide/playbooks_conditionals.html#the-when-statement


ansible_os_family": "Debian"

When condition is always used bottom of the script and using scrips we can able to run a playbook on a different platforms 

1.Debian
2.Redhat
---
- hosts: Webserver

  become: yes

  tasks:
  - name: install apache

    apt:
      name: apache2

    state: present

    update_cache: yes

    when: ansible_os_family == "Debian"  
  - name: install apache

    yum:

    name: httpd

     state: present

    when: ansible_os_family == "Redhat"




27/03/2025::
==============


In Ansible, variables are used to store values that can be referenced and used throughout your playbooks, roles, and tasks. This allows for dynamic, reusable, and flexible automation. Here’s a basic breakdown of how Ansible variables work and the different ways you can define and use them:


define variables in 3 places
1.	Inventory level  lowest priority
2.	Playbook level 
3.	Command line level –highest level priority


Inventory variables: These are defined in the inventory file (or dynamic inventory) for specific hosts or groups.

[webservers]
ansiblenode1@172.31.20.135  package_name=git
ansiblenode2@172.31.30.200 package_name=apache2
localhost 

[webservers:vars]
ansiblenode2@172.31.30.200 
localhost 

package_name=httpd

Playbook variables: You can define variables directly within your playbooks using the vars section.

---
- hosts: Webservers

  become: yes

  vars:

  pacakge_name: git

  tasks:
    
    - name: Install all packages

      apt:

      name: "{{ pacakge_name }}"

      state: present

      Command-line variables: You can pass variables to your playbooks at runtime using the -e or --extra-vars option.
      

      >ansible-playbook -i hosts -e "package_name=apache2" variables2.yml



Ansible resolves variable values based on a specific precedence order. The order from highest to lowest precedence is:
====================================================================================================================

Extra-vars (-e on the command line): Command-line variables take the highest precedence.

Playbook variables: Variables defined within the playbook.

Inventory variables: Variables set in the inventory.

Debug & vars & register in Ansible module::
==========================================

https://docs.ansible.com/ansible/latest/collections/ansible/builtin/debug_module.html

---
- name: Echo message on localhost

  hosts: localhost

   connection: local

   gather_facts: no

   vars:

   message: "Hello from Ansible playbook on localhost!"

  tasks:
    
    - name: Echo message and connection type

      ansible.builtin.shell: "echo '{{ message }}' ; echo 'Connection type: {{ ansible_connection }}'"

      register: echo_output

    
    - name: Display output

      debug:

      msg: "{{ echo_output.stdout_lines }}"


>ansible-playbook -i hosts -vvv variable.yaml  --------> verbose logs purpose ,please run this command


![image](https://github.com/user-attachments/assets/7d18a6e5-a53b-436b-bf26-dbe1db0e89af)


Registry Module::
-----------------
Registry is a module used to results can be stored in a variable
Stored ouptput of a task or script
I want execute a command and results can be stored in a variable is called registry

Handlers::
===========
Sometimes you want a task to run only when a change is made on a machine. For example, you may want to restart a service if a task updates the configuration of that service, but not if the configuration is unchanged. Ansible uses handlers to address this use case. Handlers are tasks that only run when notified

---
  hosts: webservers
  become: yes
  tasks:
    - name: Ensure apache is at the latest version
      ansible.builtin.yum:
        name: httpd
        state: latest
  handlers:
    - name: Restart apache
      ansible.builtin.service:
        name: httpd
        state: restarted


28/03/2025::
===================


Ansible Roles::
===================

Ansible roles are a way of organizing playbooks and tasks in a modular, reusable, and maintainable structure. They allow you to break down complex playbooks into smaller, focused units of functionality that can be easily shared and reused across different projects. Here's a more detailed look at Ansible roles:

https://docs.ansible.com/ansible/latest/playbook_guide/playbooks_reuse_roles.html

1.Written ansible in a reusable fashion
2.How do I use someone else’s work
3.Ansible galaxy is a place where we can find reusable roles

https://galaxy.ansible.com/

4.Which we can use in your script



install roles

 > Ansible-galaxy install <rolename>

 >ansible-galaxy install my_role

create my own role::

> ansible-galaxy init <rolename>

>ansible-galaxy init my_role



Structure of Ansible Roles::
===================

my_role/
├── defaults/
│   └── main.yml            # Default variables
├── files/
│   └── somefile            # Files to be copied to the target
├── handlers/
│   └── main.yml            # Handlers (usually for service restarts)
├── meta/
│   └── main.yml            # Metadata about the role
├── tasks/
│   └── main.yml            # The main tasks (this file includes other task files if needed)
├── templates/
│   └── config.j2           # Jinja2 templates for dynamic file creation
├── tests/
│   └── test.yml            # Test playbooks to verify the role works
├── vars/
│   └── main.yml            # Custom variables


Using Roles in Playbooks
Once you've defined a role, you can use it in your playbook like this:

---
- name: Example Playbook using roles
  hosts: all
  become: yes
  roles:
    - my_role

Benefits of Using Roles
Reusability: Roles can be reused across different playbooks and projects.

Modularity: Roles allow you to organize your playbook into smaller, manageable parts.

Clarity: Each role focuses on a specific task or function, making your playbooks more understandable.

Example Role: Installing Tomcat

https://galaxy.ansible.com/ui/standalone/roles/robertdebock/tomcat/install/


Create my own role

> Ansible-galaxy init rolename

![image](https://github.com/user-attachments/assets/af275783-63b6-40ab-a319-645db283a40f)

![image](https://github.com/user-attachments/assets/34cfe34b-b8bc-4026-9014-0c07c952c3af)

Install tomcat

If you're looking to install or use an Ansible role for Tomcat from Ansible Galaxy, you can search for available roles and collections related to Tomcat. Here's how you can find and use a role related to Tomcat from Galaxy.
1.	Search for a Tomcat Role

https://galaxy.ansible.com/

To search for a role related to Tomcat on Ansible Galaxy, you can use the following command:
bash
Copy
ansible-galaxy search tomcat
This will return a list of roles related to Tomcat that you can install and use.
2. Install a Tomcat Role
Once you’ve found a suitable role for Tomcat, you can install it using the ansible-galaxy install command.
For example, if you find a role called geerlingguy.tomcat, you can install it by running:
bash
Copy
> ansible-galaxy install geerlingguy.tomcat
This will download and install the role into your ~/.ansible/roles/ directory (or the path defined in your ansible.cfg file).
3. Use the Installed Tomcat Role in Your Playbook
After installing the role, you can use it in your playbook. Here’s an example of a simple playbook that installs and configures Tomcat:
yaml
Copy

Deploywar.yml::
=============

---
- hosts: localhost
  become: yes
  roles:
  - robertdebock.java
  - robertdebock.tomcat
 
  > ansible-playbook -i hosts Deploywar.yml
  

![image](https://github.com/user-attachments/assets/306fd1fc-8c51-40f7-81b6-41a44e6ee915)

  
This will use the geerlingguy.tomcat role to set up Tomcat on your webservers hosts.

https://galaxy.ansible.com/robertdebock/tomcat

![image](https://github.com/user-attachments/assets/29cfc5e4-b8e6-494b-a462-d8a11699df12)

Deploywar.yml

![image](https://github.com/user-attachments/assets/d7f4d510-bee2-4d32-ad56-7906a8574e93)

![image](https://github.com/user-attachments/assets/adad9ea6-ed52-457e-a9eb-adb2d19ad026)

![image](https://github.com/user-attachments/assets/a4c880aa-f378-4085-9122-3ef93a25e09a)


By default  tomcat run port 8080
http://18.236.181.244:8080/
http://34.216.173.44:8080/manager/html

![image](https://github.com/user-attachments/assets/fa5faaeb-ec9e-43f2-9184-7bf46f1433c4)


Most of the work is done 
Where is my war file

Deploy Onlinebook store war to tomcat server using roles::
==============================================================

>If war file is available in local machine use copy module
>if war file is available other machine(internet) use get_url module
Tomcat by default install

>/opt/tomcat

![image](https://github.com/user-attachments/assets/45a19e09-7641-4dec-b730-d2b01a3ea63b)

![image](https://github.com/user-attachments/assets/721d2e75-0368-4d87-bdf1-d54331ef8afb)

---
- hosts: Webservers
  become: yes
  roles:
  - robertdebock.java
  - robertdebock.tomcat
  tasks:
  - name: copy war
    get_url:
      url: https://baby7358.s3.us-west-2.amazonaws.com/onlinebookstore.zip 
      dest: /opt/tomcat/webapps/gameoflife.war


![image](https://github.com/user-attachments/assets/d43d4d4a-ee8d-4dd8-af09-b71dfdf2da6f)

Create S3 Bucket in AWS account::
===============================

Go to AWS account and search S3 bucket 

S3=SSS=simple storage services

![image](https://github.com/user-attachments/assets/8c1b5637-9392-414d-ab0b-21bf9d882609)

Select S3

![image](https://github.com/user-attachments/assets/c62a298f-185d-43ec-9d62-8b874e7627ec)

Click Create bucket

![image](https://github.com/user-attachments/assets/097eedf8-8e2f-48f5-876f-2c3debfccda8)

Bucket name provide

![image](https://github.com/user-attachments/assets/669f5b5a-d4e4-43ee-add1-e6be36171ec4)

Object Ownership  ---- ACLs enabled selected


Unchecked Block all public access


![image](https://github.com/user-attachments/assets/61cac919-cbbd-4b39-9121-d1ed20e33bcd)

Ackened 

![image](https://github.com/user-attachments/assets/9edcd3b0-c71a-4e78-8132-0469a192cd82)

Click crete bucket

![image](https://github.com/user-attachments/assets/c0b39afe-325c-4d82-9ea6-2204896c1f55)

S3 bucket is created in AWS

![image](https://github.com/user-attachments/assets/702e2185-29cd-43d2-9176-ad9788907bc8)

S3 bucket Created successfully


![image](https://github.com/user-attachments/assets/3c2855d7-ae2c-4f18-8ce7-3b766211b811)

Click Bucket

![image](https://github.com/user-attachments/assets/3000b5bc-8691-40cc-b5ee-e378fe813bf6)


Click Upload 


![image](https://github.com/user-attachments/assets/71efca18-9c4a-4bad-97ff-6e6baf6b559c)

Click Add Files


![image](https://github.com/user-attachments/assets/e74175f3-ca04-47bb-977b-9f9df1cf7139)

Select Onlinebookstore.war file

![image](https://github.com/user-attachments/assets/89cac099-5c85-4a29-91e9-8868f2e2f020)

Select check box to upload the onlinebookstore.war file

![image](https://github.com/user-attachments/assets/30c81ce3-4605-45e9-90bd-b719dac4d875)

Click Upload

![image](https://github.com/user-attachments/assets/85a5204d-b660-4d0c-8983-fc24b05427e4)

Upload Succeeded

![image](https://github.com/user-attachments/assets/11d79c2d-c353-404c-be41-130608b34dcb)

Copy URL

![image](https://github.com/user-attachments/assets/147864ff-fc89-4ae1-b104-b383cccba33b)

![image](https://github.com/user-attachments/assets/37ad0996-d054-4a3b-aa57-c0480254c1c1)

Copy url to below script:: onlinebookstore.yml
===================

---
- hosts: localhost
  become: yes
  roles:
  - robertdebock.java
  - robertdebock.tomcat
  tasks:
  - name: copy war
    get_url:
      url: https://infocus942.s3.us-west-2.amazonaws.com/onlinebookstore.war
      dest: /opt/tomcat/webapps/onlinebookstore.war

![image](https://github.com/user-attachments/assets/402272bc-6604-4840-a406-c1cc8e95dcc6)

run the playbook

>ansible-playbook -i hosts onlinebookstore.yml

![image](https://github.com/user-attachments/assets/4ed55d65-f16e-4314-8dba-c3a34c3ee5c2)

Success

![image](https://github.com/user-attachments/assets/592b947e-d422-4430-9729-98724403ce0d)

Verify deployment in Tomcat server

![image](https://github.com/user-attachments/assets/c50103d8-21ba-484e-8562-34a1b5b2c0d0)

http://54.218.133.244:8080/onlinebookstore/

![image](https://github.com/user-attachments/assets/e79ac48a-f76e-42ff-b5a5-28094402c20a)

Integrated Ansible & Tomcat & S3::
=====================================

![image](https://github.com/user-attachments/assets/77ca7c84-e2e9-41c3-a6df-e4cbe91a3e03)



01/04/2025::
================


Docker Introductions::
=================

Docker is an opensource & Applicatuions level virtualization technology and it's called containirazition.

Docker is an open-source platform that automates the deployment, scaling, and management of applications in lightweight, portable containers. Containers are isolated environments that package an application and all its dependencies (such as libraries, binaries, and configurations) to ensure it runs uniformly across different computing environments.

container ::
==============
1.container is an insolation area of executuions of your applications
 OR
 instance of images are called containers
2.Containers are created from “images”
3. Containers are the core of Docker. They are lightweight, portable, and isolated environments where applications run.
  Docker is run your software packages /Applications  in containers called containarizations.

4. if you build a docker container for your application called containerization
5. containers have it’s own boundaries  

who will create containers?
Ans --docker images are created the containers

 Docker Images:
 ===============

 docker image is a package with all dependencies and the necessary 
information to create the container and docker image derived from multiple base images.

An image is a snapshot of a container, a blueprint that defines what the container will contain and how it will behave when run. It consists of an application and its dependencies. Docker images are built using a Dockerfile

Docker Registry::
====================

A Docker Registry is a system for storing and distributing Docker images. It is a centralized location where Docker images can be uploaded (pushed), stored, and downloaded (pulled) by users and applications. Docker images are the building blocks of containers, and registries provide a way to manage, version, and share these images across different environments.

Default registry :: https://hub.docker.com/

Physical & Virtual & Hypervisors/VMwares::
=============================================

1.tomcat & nodejs containers have it’s own process tree,own files systems,own network interfaces own storage,ram…etc
2.when you want to give application to your team/testers  docker is the best choice and when you want give system to your team/ testers VMwares are best choice.
3.application level virtulization docker is the best choice and OS level virtulization VMwares are best choice
4.individually scale the your application very easy in docker

![image](https://github.com/user-attachments/assets/94a53226-77d3-402d-8a89-2e5fc7879099)


Example:: For festival season In your organization leave management application multiple employees are applied leaves at the same time in that scenario docker is very easy to scale the one more application but physically it’s very difficult so docker is the best choice




02/04/2025::
=============


Install Docker in Ubuntu machine::
=====================================

Please follow below link steps to install the docker in ubuntu and please read all the content in that link

https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04

once installed docker please verify below commands::

>docker --version

root@ip-172-31-20-86:~# docker --version
Docker version 28.0.4, build b8034c0

root@ip-172-31-20-86:~# docker info
Client: Docker Engine - Community
 Version:    28.0.4
 Context:    default
 Debug Mode: false
 Plugins:
  buildx: Docker Buildx (Docker Inc.)
    Version:  v0.22.0
    Path:     /usr/libexec/docker/cli-plugins/docker-buildx
  compose: Docker Compose (Docker Inc.)
    Version:  v2.34.0
    Path:     /usr/libexec/docker/cli-plugins/docker-compose

Server:
 Containers: 0
  Running: 0
  Paused: 0
  Stopped: 0
 Images: 0
 Server Version: 28.0.4
 Storage Driver: overlay2
  Backing Filesystem: extfs
  Supports d_type: true
  Using metacopy: false
  Native Overlay Diff: true
  userxattr: false
 Logging Driver: json-file
 Cgroup Driver: systemd
 Cgroup Version: 2
 Plugins:
  Volume: local
  Network: bridge host ipvlan macvlan null overlay
  Log: awslogs fluentd gcplogs gelf journald json-file local splunk syslog
 Swarm: inactive
 Runtimes: io.containerd.runc.v2 runc
 Default Runtime: runc
 Init Binary: docker-init
 containerd version: 05044ec0a9a75232cad458027ca83437aae3f4da
 runc version: v1.2.5-0-g59923ef
 init version: de40ad0
 Security Options:
  apparmor
  seccomp
   Profile: builtin
  cgroupns
 Kernel Version: 6.8.0-1024-aws
 Operating System: Ubuntu 24.04.2 LTS
 OSType: linux
 Architecture: x86_64
 CPUs: 2
 Total Memory: 3.82GiB
 Name: ip-172-31-20-86
 ID: 201c6f4b-75d3-4326-adf5-00b9a82a8d4d
 Docker Root Dir: /var/lib/docker
 Debug Mode: false
 Experimental: false
 Insecure Registries:
  ::1/128
  127.0.0.0/8
 Live Restore Enabled: false

if above page is came without any erros, it means docker is installed in your machine


Docker High Level Client -Server Architecture::
==================================


![image](https://github.com/user-attachments/assets/695f72c0-a316-4f55-81c9-d4eb79c59826)

Docker's high-level architecture revolves around several components that work together to provide containerization and isolation for applications


Docker Client (CLI)::
=================

The Docker Client is the primary interface for interacting with Docker. It can be a command-line interface (CLI), like the docker command, or a graphical interface (GUI) in some tools.

It allows users to interact with Docker's features, such as building containers, running containers, and managing containers and images.

It sends requests to the Docker Daemon to execute commands.

Docker Daemon (Dockerd)::
====================

The Docker Daemon (also known as dockerd) is the core component of Docker. It runs in the background on the host system.

The daemon is responsible for managing Docker containers, images, networks, and volumes. It listens for Docker API requests and handles container lifecycle operations such as starting, stopping, and building containers.

The Docker Daemon can communicate with multiple Docker clients, allowing for distributed management of containers.

Flow:
============
1.The Docker Client sends a command to the Docker Daemon.

2.The Docker Daemon interacts with containers, images, and storage volumes.

3.The Docker Daemon can pull images from a Docker Registry.

4.The Docker Daemon runs containers based on the images and handles networking and storage.

Docker commands::
====================

 >docker pull <imagename>
 >docker pull hello-world
 >docker images   ----used to display the all images
 > docker image ls ----used to display the all images
 
 >docker run ---used to build the images and create the container
>
detached mode::
=================

Docker detached mode refers to running a container in the background

>docker run -d <image_name>

example::
> docker run -d nginx

Where:

-d is the flag for detached mode.

<image_name> is the name of the Docker image you want to run.

> docker run -d nginx

This command will:

Run the nginx container in detached mode.

Start the container in the background.

To view the containers running in detached mode, you can use the docker ps command:
======================================

>docker ps

Stopping a Container::
=================

>docker stop <containerID>

Start a Container::
=================

>docker start <containerID>

To run a command inside a running container:
======================

>docker exec -it <container_id_or_name> <command>
>docker exec -it 5336d949f33b /bin/bash

>root@5336d949f33b:/# hostname
5336d949f33b
>root@5336d949f33b:/# hostname -i
172.17.0.3


![image](https://github.com/user-attachments/assets/c7114894-3fcd-46b0-b393-6f296d23b845)

NOTE:::
=========

>docker exec -it 5178eb58223a /bin/bash
Use this command inside the container

>ctrl pq
Outside the containers

Lab practice::
===============

take one nginx web server

>docker pull nginx

root@ip-172-31-20-86:~# docker pull nginx
Using default tag: latest
latest: Pulling from library/nginx
6e909acdb790: Pull complete
5eaa34f5b9c2: Pull complete
417c4bccf534: Pull complete
e7e0ca015e55: Pull complete
373fe654e984: Pull complete
97f5c0f51d43: Pull complete
c22eb46e871a: Pull complete
Digest: sha256:124b44bfc9ccd1f3cedf4b592d4d1e8bddb78b51ec2ed5056c52d3692baebc19
Status: Downloaded newer image for nginx:latest
docker.io/library/nginx:latest

>docker images

root@ip-172-31-20-86:~# docker images
REPOSITORY        TAG       IMAGE ID       CREATED        SIZE
jenkins/jenkins   latest    be95e0848c42   7 days ago     466MB
nginx             latest    53a18edff809   7 weeks ago    192MB

>docker run -d -p 80:80 nginx

root@ip-172-31-20-86:~# docker run -d -p 80:80 nginx
3d1a52d091b05878e079b89002aa57b460c5263a585a8add0ecc671608d1f999

>docker ps

root@ip-172-31-20-86:~# docker ps
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS         PORTS                                 NAMES
3d1a52d091b0   nginx     "/docker-entrypoint.…"   3 seconds ago   Up 3 seconds   0.0.0.0:80->80/tcp, [::]:80->80/tcp   thirsty_shaw

>docker exec -it 3d1a52d091b0

root@ip-172-31-20-86:~# docker exec -it 3d1a52d091b0  /bin/bash
docker: 'docker exec' requires at least 2 arguments

root@ip-172-31-20-86:~# docker exec -it 3d1a52d091b0 /bin/bash
root@3d1a52d091b0:/# hostname
3d1a52d091b0
root@3d1a52d091b0:/# hostname -i
172.17.0.3

root@5336d949f33b:/# ls
bin  boot  dev  docker-entrypoint.d  docker-entrypoint.sh  etc  home  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
root@5336d949f33b:/# cd opt/
root@5336d949f33b:/opt# ls
root@5336d949f33b:/opt# cd ..
root@5336d949f33b:/# ls
bin  boot  dev  docker-entrypoint.d  docker-entrypoint.sh  etc  home  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
root@5336d949f33b:/# cd usr/
root@5336d949f33b:/usr# ls
bin  games  include  lib  lib64  libexec  local  sbin  share  src
root@5336d949f33b:/usr# cd lib
root@5336d949f33b:/usr/lib# ls
apt  dpkg  init  locale  lsb  mime  nginx  os-release  sasl2  ssl  systemd  terminfo  tmpfiles.d  udev  x86_64-linux-gnu
root@5336d949f33b:/usr/lib#
root@5336d949f33b:/usr/lib# docker images
bash: docker: command not found
root@5336d949f33b:/usr/lib# docker imagesexit
bash: docker: command not found
root@5336d949f33b:/usr/lib# read escape sequence
root@ip-172-31-20-86:~# docker images
REPOSITORY        TAG       IMAGE ID       CREATED        SIZE
jenkins/jenkins   latest    be95e0848c42   7 days ago     466MB
nginx             latest    53a18edff809   7 weeks ago    192MB
ubuntu            latest    a04dc4851cbc   2 months ago   78.1MB
hello-world       latest    74cc54e27dc4   2 months ago   10.1kB
root@ip-172-31-20-86:~# docekr runRead from remote host ec2-34-204-17-141.compute-1.amazonaws.com: Connection reset by peer
Connection to ec2-34-204-17-141.compute-1.amazonaws.com closed.
client_loop: send disconnect: Connection reset by peer

we can see below nginx web page and nginx is running on containers

![image](https://github.com/user-attachments/assets/878995bc-58b1-4f20-982e-2d60f105891d)




03/04/2025::
=================

Dockerfile Introduction::
=================

A Dockerfile is a script containing a series of instructions on how to build a Docker image. It defines the environment and application setup, including dependencies, configurations, and the necessary steps to get your application running in a container.

dockerfile is a text file, and it have set up of all instructiuons

https://docs.docker.com/get-started/docker-concepts/building-images/writing-a-dockerfile/


Dockerfile::dockerfile is text file, and it have set up of all instructiuons
FROM nginx or ubuntu or 
LABEL "AUthor =nagaraju@gamil.com"
RUN apt update && apt-get install jenkins -y
COPY . .  ----src destnations
ADD  . . -----src destinatuion
CMD ["echo",".jar"]
ENTRYPOINT ["echo", "war"]
EXPOSE 8080,8085
ENV APP_HOME ="Ifocus SOlutions pvt ltd"
WORKDIR $APP_HOME /app
VOLUME 

Key Components of a Dockerfile:
==========================

FROM: Specifies the base image for the Docker image you're creating.
FROM ubuntu:20.04

RUN: Executes commands inside the container, often used to install dependencies.
RUN apt-get update && apt-get install -y python3

COPY or ADD: Copies files from your local machine into the container.
COPY . /app

WORKDIR: Sets the working directory for any subsequent commands in the Dockerfile.
WORKDIR /app
CMD: Specifies the command to run when a container is started from the image.
CMD ["python3", "app.py"]
EXPOSE: Defines the network ports the container will listen on at runtime.
EXPOSE 8080

ENV: Sets environment variables inside the container.
ENV APP_ENV=production
CMD & ENTRPOINT can be executed starting of the container

CMD & ENTRYPOINT Different::
===========================
--use CMD you can change the value but ENTRYPOINT not possible to change the value at the starting of the container
--CMD you can change the argument value 
--ENTRYPOINT can’t change the argument value

CMD ["echo",".jar"]
ENTRYPOINT ["echo", "war"]

CMD/ENTRYPOINT ====should have something which runs till your app is alive

Note::
=======
life time of your container -->time which your cmd/entrypont is alive

Example Dockerfile:::
==========
Here’s a simple Dockerfile example that builds a Python web app:

# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container
COPY . /app

# Install the required dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port the app runs on
EXPOSE 5000

# Define the command to run the application
CMD ["python", "app.py"]

Building and Running a Docker Image:
Once you’ve written your Dockerfile, you can build and run it using Docker commands:

Build the Docker image:

>docker build -t my-python-app .

Run the container:
>docker run -d -p 8080:8080 my-python-app

A **Dockerfile** is a script containing a series of instructions on how to build a Docker image. It defines the environment and application setup, including dependencies, configurations, and the necessary steps to get your application running in a container. Essentially, it's the blueprint for creating Docker images.

### Key Components of a Dockerfile:
1. **FROM**: Specifies the base image for the Docker image you're creating.
   ```dockerfile
   FROM ubuntu:20.04
   ```

2. **RUN**: Executes commands inside the container, often used to install dependencies.
   ```dockerfile
   RUN apt-get update && apt-get install -y python3
   ```

3. **COPY** or **ADD**: Copies files from your local machine into the container.
   ```dockerfile
   COPY . /app
   ```

4. **WORKDIR**: Sets the working directory for any subsequent commands in the Dockerfile.
   ```dockerfile
   WORKDIR /app
   ```

5. **CMD**: Specifies the command to run when a container is started from the image.
   ```dockerfile
   CMD ["python3", "app.py"]
   ```

6. **EXPOSE**: Defines the network ports the container will listen on at runtime.
   ```dockerfile
   EXPOSE 8080
   ```

7. **ENV**: Sets environment variables inside the container.
   ```dockerfile
   ENV APP_ENV=production
   ```

### Example Dockerfile
Here’s a simple Dockerfile example that builds a Python web app:

```dockerfile
# Use an official Python runtime as the base image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container
COPY . /app

# Install the required dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port the app runs on
EXPOSE 5000

# Define the command to run the application
CMD ["python", "app.py"]
```

### Building and Running a Docker Image:
Once you’ve written your Dockerfile, you can build and run it using Docker commands:

1. **Build the Docker image**:
   ```bash
   docker build -t my-python-app .
   ```

2. **Run the container**:
   ```bash
   docker run -p 5000:5000 my-python-app
   ```

The Dockerfile streamlines the process of creating consistent and reproducible environments, making it easier to deploy applications across different systems.

Example2 Dockerfile::
===================

https://github.com/ifocus7358/spring-ms/blob/master/Dockerfile

Please clone this project in ubuntu machines

root@ip-172-31-20-86:~# git clone https://github.com/ifocus7358/spring-ms.git

![image](https://github.com/user-attachments/assets/188db6f2-c5b5-419d-8824-0b9b9c6728ee)

root@ip-172-31-20-86:~# cd spring-ms/
root@ip-172-31-20-86:~/spring-ms# ls
Dockerfile  azure-pipeline.yml  azure-pipelines.yml  deploy.yaml  pom.xml  src
root@ip-172-31-20-86:~/spring-ms#

Build Image::
============
root@ip-172-31-20-86:~/spring-ms# docker image build -t springmyapp .
[+] Building 0.4s (12/12) FINISHED                                                                                      docker:default
 => [internal] load build definition from Dockerfile                                                                              0.0s
 => => transferring dockerfile: 256B                                                                                              0.0s
 => WARN: FromAsCasing: 'as' and 'FROM' keywords' casing do not match (line 1)                                                    0.0s
 => [internal] load metadata for registry.access.redhat.com/ubi8/openjdk-11:latest                                                0.3s
 => [internal] load metadata for docker.io/library/maven:3.6.3-jdk-11                                                             0.1s
 => [auth] library/maven:pull token for registry-1.docker.io                                                                      0.0s
 => [internal] load .dockerignore                                                                                                 0.0s
 => => transferring context: 2B                                                                                                   0.0s
 => [internal] load build context                                                                                                 0.0s
 => => transferring context: 2.76kB                                                                                               0.0s
 => [stage-1 1/2] FROM registry.access.redhat.com/ubi8/openjdk-11:latest@sha256:28b35eea470174a39befd8eb9250a3276b79a4f6e7dac787  0.0s
 => [stage1 1/3] FROM docker.io/library/maven:3.6.3-jdk-11@sha256:1d29ccf46ef2a5e64f7de3d79a63f9bcffb4dc56be0ae3daed5ca5542b38aa  0.0s
 => CACHED [stage1 2/3] COPY . .                                                                                                  0.0s
 => CACHED [stage1 3/3] RUN mvn clean package                                                                                     0.0s
 => CACHED [stage-1 2/2] COPY --from=stage1 target/*.jar app.jar                                                                  0.0s
 => exporting to image                                                                                                            0.0s
 => => exporting layers                                                                                                           0.0s
 => => writing image sha256:bdbbb4bbe700af425032e6a27d6909e2906677fbffce9b833d596e3f37082479                                      0.0s
 => => naming to docker.io/library/springmyapp                                                                                    0.0s

 1 warning found (use docker --debug to expand):
 - FromAsCasing: 'as' and 'FROM' keywords' casing do not match (line 1)
root@ip-172-31-20-86:~/spring-ms#

![image](https://github.com/user-attachments/assets/44c6ba1e-7322-436d-af30-4606cb484283)

create container::
===============

root@ip-172-31-20-86:~/spring-ms# docker images
REPOSITORY                  TAG       IMAGE ID       CREATED        SIZE
spring                      latest    bdbbb4bbe700   9 hours ago    410MB
springmyapp                 latest    bdbbb4bbe700   9 hours ago    410MB
srinu7358/spring-03042025   latest    bdbbb4bbe700   9 hours ago    410MB
allinstructions             latest    c2993e54968d   9 hours ago    1.17GB
<none>                      <none>    805cbec82269   9 hours ago    1.17GB
testmyownimage              latest    621f509fde33   10 hours ago   1.1GB
ifocus                      latest    381bfb89fb02   10 hours ago   1.1GB
srinu7358/ifocus-myapp      latest    381bfb89fb02   10 hours ago   1.1GB
root@ip-172-31-20-86:~/spring-ms# docker run -d -p 8081:8081 springmyapp:latest
17ac78f05de4abdca3d46972e63f29c897a011d732ca3e76e7c1ef2158af10b1
root@ip-172-31-20-86:~/spring-ms#

![image](https://github.com/user-attachments/assets/d0132046-021c-46b7-9259-75382dc155fb)

![image](https://github.com/user-attachments/assets/b9064110-355c-4619-adf5-fb9fac875b6f)

Image formate::
============

<registoryname>/repositoryname:<imagetag>
Docker.io            username/reponame  ::latest

[docker.io/srinu7358/ifocus-myapp] :latest  ---->image formate

docker.io -----registry name  ----docekr hub

srinu7358 ----repository username

ifocus-myapp ---image name

>docker container run –d –p 8080:8080 springmyapp:1.0
-d --> detached mode
-p  -->mappimg a port
8080: host port
8080: container port
springmyapp:: image name
1.0:: tag name




04/04/2025:::
====================


Network Types in Docker:
============================

•	bridge: Default network for containers on the same host.
•	host: The container shares the host’s networking stack.
•	overlay: Used for multi-host networking (requires Docker Swarm).
•	none: No network connectivity is assigned to the container.
•	>bridge network is used for single node communication
•	>overlay network is used for multi node communication
•	---Kubernetes/swarm are used to communicate 2 containers in docker that’s like orchestration
macvlan network:: may be used to give containers across different hosts unique, routable IP addresses in a larger network
IPVLAN:Containers share the host’s MAC address but have individual IP addresses.

create my own network ::
=========================
> docker network create my_custom_network

![image](https://github.com/user-attachments/assets/43dbaed8-eb30-45ad-8df3-6cd9f1a3d063)

Created my own network - my_custom_network
![image](https://github.com/user-attachments/assets/a2136223-4a9a-48bc-b884-3e64a57268d5)

Run Containers on the Custom Network::
=================
>docker run -d --name container1 --network my_custom_network nginx

![image](https://github.com/user-attachments/assets/0f65c683-0ef5-4415-9413-41a46735a633)

>docker run -d --name container2 --network my_custom_network redis


![image](https://github.com/user-attachments/assets/0a4811c8-24cf-400a-93f9-e72196d504a5)

In this example:
•	container1 will run an Nginx container.
•	container2 will run a Redis container.

Both containers are connected to the my_custom_network.

Inspect the Network::
=================
To view detailed information about a network (like connected containers and settings), use the docker network inspect command:
>docker ps
>docker network ls
> docker network inspect my_custom_network

![image](https://github.com/user-attachments/assets/367d1d82-51e3-43fa-88c0-5a8414c73688)

Connect a Container to a Network:
==================
> docker network connect my_custom_network container_name
Disconnect a Container from a Network:
> docker network disconnect my_custom_network container_name
Remove a Docker Network::
>docker network rm my_custom_network
Note that the network must be unused by any containers before it can be removed.

A common use case for Docker networks is to isolate different applications or microservices, ensuring that containers in one application cannot easily communicate with containers in another. This helps you maintain security and control over how containers interact with each other.

USE CASE::
======================

--default network bridge can only ping throw ip address not container name
--our own network bridge(mybridge) able to ping both ip address and container name that’s advantage of network create.


---Kubernetes/swarm are used to communicate 2 containers in docker that’s like orchestration
--if you create your own bridge network the advantage is you can able to resolved the any issues using container name not only ipaddress but by default using you can able to resolved the issues by ipaddress.

>bridge network is used for single node communication
>overlay network is used for multi node communication


Docker Swarm::
===================

Docker and Docker Swarm are both tools used to manage containers, but they serve different purposes and have different features. 

Docker::
===========

Docker is a platform that allows you to create, deploy, and run applications inside containers. Containers are lightweight, portable, and ensure that the application works the same regardless of where it's deployed, making Docker a powerful tool for developing, testing, and deploying applications.


Key Features of Docker:
=======================
•	Containerization: Docker encapsulates applications and their dependencies into containers, ensuring consistency across environments (e.g., development, staging, production).
•	Images and Containers: Docker uses images to define the environment for an application. Containers are instances of those images.
•	Docker Hub: Docker Hub is a cloud-based registry where you can find pre-built images or upload your own.
•	Portability: Docker containers can run on any system with Docker installed, from your laptop to a cloud server.
•	Isolation: Containers are isolated from the host system, so they don’t interfere with other processes or systems.

Common Docker Commands:
===================
•	Build an Image: docker build -t my-image .
•	Run a Container: docker run -d --name my-container my-image
•	List Containers: docker ps
•	Stop a Container: docker stop my-container
•	Remove a Container: docker rm my-container
•	List Images: docker images

Docker Swarm::
==================

Docker Swarm is a clustering and orchestration tool for Docker containers. It allows you to deploy and manage multiple containers across multiple Docker hosts (machines), forming a swarm. This means that you can treat a collection of Docker hosts as a single virtual host and manage them as one.
Docker Swarm makes it easier to scale, deploy, and maintain containerized applications in production environments. It provides high availability, fault tolerance, and easy scaling of applications across multiple machines.

Key Concepts in Docker Swarm:
===============================
•	Node: A machine (physical or virtual) running Docker that is part of the Swarm cluster. There are two types of nodes:
o	Manager Node: Manages the cluster and orchestrates services.
o	Worker Node: Runs the actual containers based on instructions from manager nodes.
•	Service: A service is a description of the tasks (containers) you want to run. When you define a service, Docker Swarm ensures that the desired number of replicas of that service are running at all times.
•	Task: A task is a running container in the context of a service. Each task runs a container that is part of a service.

Docker vs Docker Swarm::
============================
•	Docker is used to build and run containers on a single machine, whereas Docker Swarm extends Docker to manage containers across a cluster of machines.
•	Docker Swarm provides orchestration features such as load balancing, scaling, and high availability, which are not available in basic Docker.
•	Docker Swarm is built into Docker, making it easier to set up and use compared to other container orchestration systems like Kubernetes.


I have created 2 ubuntu machines::
================================

1.Manager Node
2.Worker Node

![image](https://github.com/user-attachments/assets/8d70d3eb-1df0-46a0-bbae-fa9474112b8f)

>docker swarm init runs on master
>docker swarm join runs on node

> docker swarm join --token SWMTKN-1-33cj3h7mhtq98iy5aifyy9s1cdqnzh4jgl3rdgdez0vbfx8fnc-bu27q63wt2i7qfgkh0r07o85o 172.31.24.64:2377

![image](https://github.com/user-attachments/assets/c3434137-924b-4ea7-9a3f-24f188d3d19a)

![image](https://github.com/user-attachments/assets/015201ed-aea1-461f-90bc-08c1d78fae7b)

![image](https://github.com/user-attachments/assets/06424e51-1f9b-46e3-89af-80062ccb2f26)

>once initialize the swarm it will automatically created overlay network

![image](https://github.com/user-attachments/assets/d19378c2-01c9-4698-ad1d-c8af6aff1a55)


create our own overlay network ::
==========================

>docker network create –d overlay qt-overlay

![image](https://github.com/user-attachments/assets/84319ff3-e569-40c5-bdf6-69634bf65484)

> docker network create -d overlay qt-overlay
>docker node ls

![image](https://github.com/user-attachments/assets/3fb48730-74d2-4e65-ac80-dce537b2438a)

![image](https://github.com/user-attachments/assets/c545c853-157b-484f-8b7b-e3c81236d142)

create service under the overlay network::
========================

> docker service create --name my-web-service --replicas 3 -p 80:80 nginx
>docker service ls
>docker node ls

--docker always maintain --replicas 3 means 3 containers by default if for example 1 container die docker automatically create container automatically this is main use of services with docker

docker swarm:: multi containarization for your applications

Docker Swarm is a built-in container orchestration tool that allows you to manage a cluster of Docker hosts as a single entity

in any cloud we have docker /container services lke

1.AWS --->ECS ----elastic conatienr services
2.Azure---->ACS  ----Azure contaienr services
3.Kuberneties---->EKS  ---Elsatic kuberneties services


Docker compose::
====================

Docker Compose is a tool for defining and running multi-container Docker applications. With Compose, you can define all the services, networks, and volumes that your application needs in a single file (docker-compose.yml), and then run it with a single command.

Key Concepts in Docker Compose::
==============================

Service: A service is a container that runs a specific application, e.g., a web app or database. In the docker-compose.yml file, each service is defined along with its configuration (image, ports, volumes, etc.).

Network: Docker Compose automatically creates a default network for all services in your docker-compose.yml file, allowing them to communicate with each other by name. You can define additional custom networks as needed.

Volume: Volumes are used for persistent storage. For example, you may want to store database data between container restarts. Volumes are defined in the docker-compose.yml and can be shared across services.

Benefits of Using Docker Compose::
====================================

Simplified Configuration: Instead of managing multiple docker run commands and configurations, you can manage everything in a single YAML file.

Easy to Use: With a single command (docker-compose up), you can start all the services and bring up the entire environment.

Reproducibility: Since the configuration is defined in a file, you can share the same environment across different developers or servers.

Version Control: You can check the docker-compose.yml file into version control to track changes to the application's environment.

Networking & Volumes: Compose automatically sets up networking between containers and shared volumes.

Define the Application in a docker-compose.yml File::
=======================================


The docker-compose.yml file is the configuration file where you define the services, networks, and volumes. Here's a basic example for a web application using NGINX and a MySQL database:

docker-compose.yml::
======================

version: '3.8'  # Docker Compose file version

services:
  web:
    image: nginx:latest
    ports:
      - "8080:80"
    volumes:
      - ./html:/usr/share/nginx/html
    networks:
      - mynetwork

  db:
    image: mysql:latest
    environment:
      MYSQL_ROOT_PASSWORD: example
    volumes:
      - db_data:/var/lib/mysql
    networks:
      - mynetwork

volumes:
  db_data:

networks:
  mynetwork:
    driver: bridge


Explanation:
======================

services: Defines two services—web and db.
===============================

The web service uses the nginx:latest image, binds port 8080 on the host to port 80 in the container, and mounts a volume ./html to the container's /usr/share/nginx/html directory.

The db service uses the mysql:latest image and sets an environment variable for the MySQL root password. It also mounts a volume db_data to store MySQL data persistently.

Both services are connected to the same network mynetwork.

Starting the Application
=========================

Once you have your docker-compose.yml file ready, navigate to the directory containing the file and run the following command to start all the services defined in the Compose file:
please run the below command to start the docker conpose file

>docker-compose up

This will pull the images (if not already available) and start the containers.

To run it in the background (detached mode), use the -d flag:

>docker-compose up -d

Commonly Used Docker Compose Commands::
=======================================

docker-compose up: Build, (re)create, start, and attach to containers for a service.

docker-compose up -d: Run containers in detached mode (in the background).

docker-compose down: Stop and remove all containers, networks, and volumes defined in the docker-compose.yml file.

docker-compose build: Build or rebuild the services in the background.

docker-compose logs: View logs from the services.

docker-compose ps: View the status of the services and containers.

docker-compose exec: Execute commands in a running container (e.g., docker-compose exec web bash).

docker-compose stop: Stop services without removing containers.

docker-compose start: Start services that were stopped with docker-compose stop.

docker-compose restart: Restart services.



07/04/2025::
===================



Docker SWARM Overview::
=====================
- this is Docker Inc's Container Orchestration Platform
- it only supports managing Docker containerized application workloads
- it is pretty easy to install and learn
- can be installed on a laptop with pretty basic configuation as well as it is very light weight
- good for POC or learning purpose
- not production grade


Kubernetes Overview::
=========

Kubernetes (often abbreviated as K8s) is an open-source container orchestration platform designed to automate the deployment, scaling, and management of containerized applications. Originally developed by Google.

free and opensource container orchestration platform developed by Google along with many open source contributors
- it is production grade
- free for personal and commercial use
- as it is opensource, we won't get support from Google
- only supports command line interface (CLI)
- doesn't support web console
- Kubernetes does provide some basic Dashboard but it is considered a security vulnerability, hence no one uses the Kubernetes Dashboard
- Rancher is opensource webconsole for Google Kubernetes

- supports inbuilt monitoring features
  - it can check the health of our application, when it finds your application is not responding, it can repair it or replace it with another good healthy instance of your application
  - it supports inbuilt load-balancing
 
  Master ---Management --(Orchestration)
  Node machine (minion) --workers (containers)

   POD ---the smallest unit, mainatained one or more containers

  YAML --key-value paires


1.Container Orchestration: Kubernetes helps you manage multiple containers, ensuring that they run efficiently and reliably across many servers.
2.Scaling: Kubernetes can automatically scale your applications up or down based on demand, making it easier to handle varying workloads.
3.Load Balancing: It can distribute network traffic to different containers, ensuring that applications remain responsive even under heavy loads.
4.Self-Healing: If a container crashes or stops working, Kubernetes can automatically restart or replace it, ensuring the application stays available.
5.Automated Deployment and Rollback: Kubernetes can automate the process of deploying new versions of an application, and if something goes wrong, it can roll back to a previous version.
6.Storage Management: Kubernetes can automatically mount the storage resources you need for your applications, making it easier to manage persistent data.

In short, Kubernetes is designed to make it easier to manage applications at scale in a way that is highly automated, reliable, and efficient. It’s widely used in DevOps platform

Cluster:: collection of nodes with a single responsibility
All the nodes in that cluster do same process, same type of work can will do collection of nodes in cluster

Cluster::
============
a cluster might refer to a set of virtual machines or containers working together for a specific application or service.

Kubernetes Cluster Components:
===============================

1.Master Node (Control Plane):
The Master Node is the brain of the Kubernetes cluster. It manages the cluster and makes decisions about scheduling, scaling, and maintaining the health of the application. The control plane consists of several key components:

1.API Server::
==================

The API server exposes the Kubernetes API, which is used to interact with the cluster.

2.Scheduler::
============
The scheduler assigns work (pods) to available worker nodes.

3.Controller Manager: :
===================
Ensures that the desired state of the system is maintained, such as ensuring that the correct number of pods are running.

4.etcd: 
===========
A distributed key-value store used to store all cluster data, including the state of the system (like deployed pods, config maps, and secrets).

Worker Nodes (Minions):
==================
o	The Worker Nodes are responsible for running the actual application workloads. These nodes host the pods, which are the smallest deployable units in Kubernetes. A worker node typically runs:
1.Kubelet: An agent that ensures the containers in the pods are running and healthy.
2.Kube Proxy: A network proxy that maintains network rules for pod communication.
3.Container Runtime: The software responsible for running containers (e.g., Docker, containerd).
4.Pods::
A pod is the smallest unit of execution in Kubernetes and can contain one or more containers that share resources such as networking and storage. Pods are always deployed in a Kubernetes cluster and are managed by the control plane.

5.Services:
A service in Kubernetes is a way to expose an application running in a pod to other pods or external users. It ensures that network communication between pods is reliable, even as pods are dynamically created or destroyed.

NOTE:::In kubernetes master is not created containers, this is recommended approaches we can create containers in master also but not proposed

kubernetes is help to individually scale micro services

Basically, kubernetes is used for to maintain containers



08/04/2025::
==================


![image](https://github.com/user-attachments/assets/16f6dbce-164f-4b56-8922-0614eb8a779d)

Above picture directly using pods without using services and if ipaddress no longer available our application is not worked. pods communication throw ip address right, so it has a problem to resolved the this problem services is come to the picture.

Services –logical entity and maintain ip address

Below picture is running the pods with Service

![image](https://github.com/user-attachments/assets/f045db00-2883-4407-ac5d-0dd83e3129c2)


Docker and kubernetes::
=====================

Create one ubuntu machin in AWS

install docker link::
https://www.linuxtechi.com/install-use-docker-on-ubuntu/

>systemctl status docker
>docker version

Install minikube::
=====================

For that use case you can use minikube: a ONE Node cluster, where the master and worker processes are on the same machine. Minikube is a lightweight Kubernetes implementation that creates a VM on your local machine and deploys a simple cluster containing only one node
Kubectl:: Kubectl, the command line tool for Kubernetes, then enables the interaction with the cluster: to create pods, services and other components
In Kubernetes, kubectl, kubeadm, and kubelet are important tools for managing and working with a Kubernetes cluster

•	kubectl: Command-line tool for managing and interacting with Kubernetes clusters.
•	kubeadm: Tool to initialize and manage Kubernetes clusters, handling cluster setup and node joining.
•	kubelet: Node agent that ensures containers are running as expected and reports back to the control plane

Kubernetes (sometimes shortened to K8s with the 8 standing for the number of letters between the “K” and the “s”) is an open source system to deploy, scale, and manage containerized applications anywhere.

Install minikube in Ubuntu machine::
===========================
please follow below link steps to install minikube in ubuntu machine

https://www.linuxtechi.com/how-to-install-minikube-on-ubuntu/


root@ip-172-31-36-154:~# minikube start docker --force
* minikube v1.35.0 on Ubuntu 24.04 (xen/amd64)
! minikube skips various validations when --force is supplied; this may lead to unexpected behavior
* Automatically selected the docker driver. Other choices: none, ssh
* The "docker" driver should not be used with root privileges. If you wish to continue as root, use --force.
* If you are running minikube within a VM, consider using --driver=none:
*   https://minikube.sigs.k8s.io/docs/reference/drivers/none/
* Using Docker driver with root privileges
* Starting "minikube" primary control-plane node in "minikube" cluster
* Pulling base image v0.0.46 ...
* Downloading Kubernetes v1.32.0 preload ...
    > preloaded-images-k8s-v18-v1...:  333.57 MiB / 333.57 MiB  100.00% 64.47 M
    > gcr.io/k8s-minikube/kicbase...:  500.27 MiB / 500.31 MiB  99.99% 69.75 Mi
* Creating docker container (CPUs=2, Memory=2200MB) ...
* Preparing Kubernetes v1.32.0 on Docker 27.4.1 ...
  - Generating certificates and keys ...
  - Booting up control plane ...
  - Configuring RBAC rules ...
* Configuring bridge CNI (Container Networking Interface) ...
* Verifying Kubernetes components...
  - Using image gcr.io/k8s-minikube/storage-provisioner:v5
* Enabled addons: storage-provisioner, default-storageclass
* Done! kubectl is now configured to use "minikube" cluster and "default" namespace by default

root@ip-172-31-36-154:~# sudo kubectl cluster-info
Kubernetes control plane is running at https://192.168.49.2:8443
CoreDNS is running at https://192.168.49.2:8443/api/v1/namespaces/kube-system/services/kube-dns:dns/proxy

To further debug and diagnose cluster problems, use 'kubectl cluster-info dump'.

root@ip-172-31-36-154:~# kubectl get nodes
NAME       STATUS   ROLES           AGE    VERSION
minikube   Ready    control-plane   114s   v1.32.0

Clone the Project::
=====================

>git clone https://github.com/ifocus7358/docker-Java-kubernetes-project.git

root@ip-172-31-36-154:~# git clone https://github.com/ifocus7358/docker-Java-kubernetes-project.git
Cloning into 'docker-Java-kubernetes-project'...
remote: Enumerating objects: 156, done.
remote: Counting objects: 100% (42/42), done.
remote: Compressing objects: 100% (32/32), done.
remote: Total 156 (delta 27), reused 10 (delta 10), pack-reused 114 (from 1)
Receiving objects: 100% (156/156), 27.40 KiB | 9.13 MiB/s, done.
Resolving deltas: 100% (35/35), done.

Build the image::
============

root@ip-172-31-36-154:~# ls
docker-Java-kubernetes-project  minikube-linux-amd64  snap
root@ip-172-31-36-154:~# cd docker-Java-kubernetes-project/
root@ip-172-31-36-154:~/docker-Java-kubernetes-project# ls
README.md  kubernetes  productcatalogue  shopfront  stockmanager
root@ip-172-31-36-154:~/docker-Java-kubernetes-project# cd kubernetes/
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/kubernetes# ls
productcatalogue-service.yaml  shopfront-service.yaml  stockmanager-service.yaml
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/kubernetes# cd ..
root@ip-172-31-36-154:~/docker-Java-kubernetes-project# ls
README.md  kubernetes  productcatalogue  shopfront  stockmanager
root@ip-172-31-36-154:~/docker-Java-kubernetes-project# cd shopfront/
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# ls
Dockerfile  pom.xml  src
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront#
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker build -t shopfront .

installed maven::
===========

root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# mvn -v
Apache Maven 3.8.7

So need to build the source code first it will generate target folder
>mvn clean install


[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  5.598 s
[INFO] Finished at: 2025-04-08T05:52:09Z
[INFO] ------------------------------------------------------------------------
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# ls
Dockerfile  pom.xml  src  target
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# cd  target/
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront/target# ls
classes  generated-sources  maven-archiver  maven-status  shopfront-0.0.1-SNAPSHOT.jar  shopfront-0.0.1-SNAPSHOT.jar.original
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront/target# ls
classes  generated-sources  maven-archiver  maven-status  shopfront-0.0.1-SNAPSHOT.jar  shopfront-0.0.1-SNAPSHOT.jar.original
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront/target# cd ..
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker build -t shopfront .
[+] Building 8.8s (7/7) FINISHED                                                                                        docker:default
 => [internal] load build definition from Dockerfile                                                                              0.0s
 => => transferring dockerfile: 198B                                                                                              0.0s
 => [internal] load metadata for docker.io/library/openjdk:8-jre                                                                  0.1s
 => [internal] load .dockerignore                                                                                                 0.0s
 => => transferring context: 2B                                                                                                   0.0s
 => [internal] load build context                                                                                                 0.5s
 => => transferring context: 46.10MB                                                                                              0.5s
 => [1/2] FROM docker.io/library/openjdk:8-jre@sha256:667a15e7bc533a90fb39ddb7e5bed63162ac3c13a97e6c698bf4f139f51b7d33            6.1s
 => => resolve docker.io/library/openjdk:8-jre@sha256:667a15e7bc533a90fb39ddb7e5bed63162ac3c13a97e6c698bf4f139f51b7d33            0.0s
 => => sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a 10.88MB / 10.88MB                                  0.3s
 => => sha256:a6a74c7b774e00fd2ec5664e257d344f1b7e69e2a618b1c0678f69719863c5ad 1.58kB / 1.58kB                                    0.0s
 => => sha256:0c14a0e20aa3a19448f6227265c6642571112e9cd9a69b5e7a323df46d1aa835 7.43kB / 7.43kB                                    0.0s
 => => sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165 5.16MB / 5.16MB                                    0.2s
 => => sha256:667a15e7bc533a90fb39ddb7e5bed63162ac3c13a97e6c698bf4f139f51b7d33 1.04kB / 1.04kB                                    0.0s
 => => sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452 55.00MB / 55.00MB                                  1.3s
 => => sha256:8510da692cda60e4746c14dd90905695eade5888e2ad640706a2be9dc42a0224 5.66MB / 5.66MB                                    0.5s
 => => sha256:c34215579d03c1311f4e8cd3525bc03dbbb53d79d8b58e63cce8cdd355356347 211B / 211B                                        0.4s
 => => sha256:73d77b4774a96dfa09076212d5170e977d153ceab60c1ec4312a8f436b91371c 41.42MB / 41.42MB                                  1.2s
 => => extracting sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452                                         2.7s
 => => extracting sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165                                         0.2s
 => => extracting sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a                                         0.3s
 => => extracting sha256:8510da692cda60e4746c14dd90905695eade5888e2ad640706a2be9dc42a0224                                         0.2s
 => => extracting sha256:c34215579d03c1311f4e8cd3525bc03dbbb53d79d8b58e63cce8cdd355356347                                         0.0s
 => => extracting sha256:73d77b4774a96dfa09076212d5170e977d153ceab60c1ec4312a8f436b91371c                                         1.0s
 => [2/2] ADD target/shopfront-0.0.1-SNAPSHOT.jar app.jar                                                                         2.1s
 => exporting to image                                                                                                            0.3s
 => => exporting layers                                                                                                           0.3s
 => => writing image sha256:3ccf19de392942c193c580caabe914257071f0c0b1cb8c8b371d369d5e0630fd                                      0.0s
 => => naming to docker.io/library/shopfront                                                                                      0.0s
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker images
REPOSITORY                    TAG       IMAGE ID       CREATED          SIZE
shopfront                     latest    3ccf19de3929   14 seconds ago   320MB
gcr.io/k8s-minikube/kicbase   v0.0.46   e72c4cbe9b29   2 months ago     1.31GB
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker run -d -p 80:80 shopfront
836d8e23016935ac3cd74067bbdb4998dba147ce425d17edafced967b1884233
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker ps
CONTAINER ID   IMAGE                                 COMMAND                  CREATED          STATUS          PORTS                                                                                                                                  NAMES
836d8e230169   shopfront                             "java -Djava.securit…"   6 seconds ago    Up 5 seconds    0.0.0.0:80->80/tcp, [::]:80->80/tcp, 8010/tcp                                                                                          epic_leavitt
ad8f297fbeca   gcr.io/k8s-minikube/kicbase:v0.0.46   "/usr/local/bin/entr…"   27 minutes ago   Up 27 minutes   127.0.0.1:32768->22/tcp, 127.0.0.1:32769->2376/tcp, 127.0.0.1:32770->5000/tcp, 127.0.0.1:32771->8443/tcp, 127.0.0.1:32772->32443/tcp   minikube
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront#
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker images
REPOSITORY                    TAG       IMAGE ID       CREATED         SIZE
shopfront                     latest    3ccf19de3929   3 minutes ago   320MB
gcr.io/k8s-minikube/kicbase   v0.0.46   e72c4cbe9b29   2 months ago    1.31GB
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker ps
CONTAINER ID   IMAGE                                 COMMAND                  CREATED              STATUS              PORTS                                                                                                                                  NAMES
836d8e230169   shopfront                             "java -Djava.securit…"   About a minute ago   Up About a minute   0.0.0.0:80->80/tcp, [::]:80->80/tcp, 8010/tcp                                                                                          epic_leavitt
ad8f297fbeca   gcr.io/k8s-minikube/kicbase:v0.0.46   "/usr/local/bin/entr…"   28 minutes ago       Up 28 minutes       127.0.0.1:32768->22/tcp, 127.0.0.1:32769->2376/tcp, 127.0.0.1:32770->5000/tcp, 127.0.0.1:32771->8443/tcp, 127.0.0.1:32772->32443/tcp   minikube
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker rm 836d8e230169
Error response from daemon: cannot remove container "/epic_leavitt": container is running: stop the container before removing or force remove
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker rm -f 836d8e230169
836d8e230169
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker ps
CONTAINER ID   IMAGE                                 COMMAND                  CREATED          STATUS          PORTS                                                                                                                                  NAMES
ad8f297fbeca   gcr.io/k8s-minikube/kicbase:v0.0.46   "/usr/local/bin/entr…"   29 minutes ago   Up 29 minutes   127.0.0.1:32768->22/tcp, 127.0.0.1:32769->2376/tcp, 127.0.0.1:32770->5000/tcp, 127.0.0.1:32771->8443/tcp, 127.0.0.1:32772->32443/tcp   minikube
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker images
REPOSITORY                    TAG       IMAGE ID       CREATED         SIZE
shopfront                     latest    3ccf19de3929   4 minutes ago   320MB
gcr.io/k8s-minikube/kicbase   v0.0.46   e72c4cbe9b29   2 months ago    1.31GB
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker image tag shopfront srinu7358/shopfront-myapp
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker images
REPOSITORY                    TAG       IMAGE ID       CREATED         SIZE
shopfront                     latest    3ccf19de3929   6 minutes ago   320MB
srinu7358/shopfront-myapp     latest    3ccf19de3929   6 minutes ago   320MB
gcr.io/k8s-minikube/kicbase   v0.0.46   e72c4cbe9b29   2 months ago    1.31GB
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker login -u srinu7358

i Info → A Personal Access Token (PAT) can be used instead.
         To create a PAT, visit https://app.docker.com/settings


Password:

WARNING! Your credentials are stored unencrypted in '/root/.docker/config.json'.
Configure a credential helper to remove this warning. See
https://docs.docker.com/go/credential-store/

Login Succeeded
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker push srinu7358/shopfront-myapp
Using default tag: latest
The push refers to repository [docker.io/srinu7358/shopfront-myapp]
c54136e18c64: Pushed
1aaddf64804f: Mounted from library/openjdk
990c5138f5d1: Mounted from library/openjdk
5c384ea5f752: Mounted from library/openjdk
293d5db30c9f: Mounted from library/openjdk
03127cdb479b: Mounted from library/openjdk
9c742cd6c7a5: Mounted from library/openjdk
latest: digest: sha256:e027803e479a98c9d1fdcc6d983a6b778b62c2a91dee9bcccfffcb921848b42e size: 1794
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker pull srinu7358/shopfront-myapp:latest
latest: Pulling from srinu7358/shopfront-myapp
Digest: sha256:e027803e479a98c9d1fdcc6d983a6b778b62c2a91dee9bcccfffcb921848b42e
Status: Image is up to date for srinu7358/shopfront-myapp:latest
docker.io/srinu7358/shopfront-myapp:latest
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# docker images
REPOSITORY                    TAG       IMAGE ID       CREATED          SIZE
shopfront                     latest    3ccf19de3929   12 minutes ago   320MB
srinu7358/shopfront-myapp     latest    3ccf19de3929   12 minutes ago   320MB
gcr.io/k8s-minikube/kicbase   v0.0.46   e72c4cbe9b29   2 months ago     1.31GB
root@ip-172-31-36-154:~/docker-Java-kubernetes-project/shopfront# cd ..
root@ip-172-31-36-154:~/docker-Java-kubernetes-project# ls
README.md  kubernetes  productcatalogue  shopfront  stockmanager
root@ip-172-31-36-154:~/docker-Java-kubernetes-project# Read from remote host ec2-54-174-108-84.compute-1.amazonaws.com: Connection reset by peer
Connection to ec2-54-174-108-84.compute-1.amazonaws.com closed.
client_loop: send disconnect: Connection reset by peer

pushed image to docker hub::
----------------------

![image](https://github.com/user-attachments/assets/4223faf9-b478-4d75-8f4e-7c7017d52e7b)



09/04/2025::
=============

Discussed all doubts and clarification

