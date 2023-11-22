# Understanding and using GitHub Codespaces
## Session labs for codespace only
## Revision 1.1 - 11/22/23

**NOTE: To copy and paste in the codespace, you can use keyboard commands - CTRL+C and CTRL+V, or, if you want to use the mouse to copy and paste, hold the SHIFT key while copying/pasting text.**

**Lab 1 - Exploring Codespaces**

**Purpose: In this lab, we’ll start to learn our way around a codespace.**

1. Take a look around your codespace.  In the "Activity Bar" on the left, click on the various icons to see the different fuctionality of each. Don't forget about the two icons at the bottom left for "Accounts" and "Manage".

![Exploring activity bar](./images/spaces4.png?raw=true "Exploring activity bar")
![Exploring activity bar](./images/spaces5.png?raw=true "Exploring activity bar")
  
2. Go back to the Explorer icon at the top of the Activity Bar and click on that. Click on the "> extra" item to expand that and then click on the top file there 'registry-compose.yml' to open it up. [version](https://github.com/skillrepos/cspaces/blob/1984227b82fc06e1907f1f3073178d8a469ad203/extra/registry-compose.yml)

![Opening a file](./images/spaces6.png?raw=true "Opening a file")

3. Since we have two files, let's change the editors to be side-by-side.  Click on the tab above the file name and drag it over to the far side where it starts to go just off of the window.  Release the tab and it should drop into a side-by-side editor view.

![Change to split editor](./images/spaces7.png?raw=true "Change to split editor")
![Split editor](./images/spaces8.png?raw=true "Split editor")
  
4. Next, let's see another way to open files from the terminal. In your terminal session, enter the following:  
```
code roar-k8s/roar-complete.yaml
```
This should open up that file in another tab as shown below.

![Opening a file #2](./images/spaces9.png?raw=true "Opening a file #2")

5. Now. let's see how to compare two files.  Select the 'roar-complete.yaml' file and right-click and choose 'Select for Compare'. 

![Selecting files to compare](./images/spaces10.png?raw=true "Selecting files to compare")
   
6. Now, select the 'roar-complete.yaml.configmap' file, right-click and select "Compare with Selected".

![Selecting files to compare](./images/spaces11.png?raw=true "Selecting files to compare")

7. At this point, you should see the comparison file shown as a new editor tab. You can right click on any line to see options for making changes. You can drag the small gray block to scroll through differences (#1 in figure below) and then close it by clicking on the "x" in the tab (#2 in the figure below).

![Comparing files](./images/spaces12.png?raw=true "Comparing files")

8. Let's look at one more way to compare files from the terminal. First, let's create a second terminal. You can do that in multiple ways - by selecting the two column icon (A in figure below), by clicking on the "+" option (#2 in the figure below) by using a keyboard shortcut, or by right-clicking and selecting "Split Terminal"(C in figure below).  We'll use the last approach.  Right-click in the terminal and select "Split terminal".

![Splitting terminal](./images/spaces13.png?raw=true "Splitting terminal")

9. After this, you'll have two side-by-side terminals. To the far right, you'll have a list of terminals and if you hover over the bash command entry, you can see the running process info.

![Split terminal](./images/spaces14.png?raw=true "Split terminal")

10. In your new terminal start typing 'code -d'. Then, let's swap the right terminal with the left. Hover over the terminal list and drag the bottom (right) one up over the top (left) one.  After you're done, you can drag the dividing line to make more room in the left-hand session.

![Swapping terminals](./images/spaces15.png?raw=true "Swapping terminals")

11. Click on the 'roar-complete.yaml.configmap' file on the left and drag it over and drop it next to the 'code -d' command.

![Comparing file 1](./images/spaces16.png?raw=true "Comparing file 1")

12. **Type at least one space after the first file name.**  Now do the same "drag and drop" for the 'roar-complete.yaml' file, selecting it and dropping it after the other file and the spaces.

![Comparing file 2](./images/spaces17.png?raw=true "Comparing file 2")


13. When you hit return, you should see the same kind of diff as you did before.  Suppose we want to get a "longer" view of this file to see more of the differences. We can click on the "Toggle panel" button to see that.

![Toggled view](./images/spaces18.png?raw=true "Toggled view")

14. Click on the same toggle panel button again to get back to the normal view and see the terminal again.  You can click the "x" on the diff to close that. (Optional) If you want, you can delete one of the two terminal sessions by clicking on the trashcan icon over in the terminal list to the right.

![Delete terminal](./images/spaces19.png?raw=true "Delete terminal")

<p align="center">
**[END OF LAB]**
</p>

**Lab 2 - Customizing Codespaces**

**Purpose: In this lab, we’ll see how to customize a codespace.**

1. Let's install an extension for the color theme in the codespace. For practice, we'll install the "Winter is Coming Theme." Click on the Extensions icon (#1 in figure below), then in the search bar type in "winter" to quickly find the extension (#2).

 
![Find extension](./images/spaces20.png?raw=true "Find extension")

2. Once found, you can directly install the extension (#3 in figure below) or click on it (#1) and bring up the info in an editor page and scroll around it (#2) to get more details.  Go ahead and install it when ready.

![Install extension](./images/spaces21.png?raw=true "Find extension")

3. After installing, you'll see a list where you can select one of the new color themes. You can choose another one from the list if desired.

![Theme list](./images/spaces22.png?raw=true "Theme list")

4. While we're here, let's install the "GitLens" extension to allow us to more easily get Git info in the codespace.  Click on the extensions icon, search for "GitLens" and install as before.

![Installing GitLens](./images/spaces23.png?raw=true "Installing GitLens")

5. After this, you'll have new icons in the Activity Bar related to GitLens. If you select a line in an editor, you can see information next to it about the commit in Git that led to it.  And hovering over it gives you more information.

![GitLens in use](./images/spaces24.png?raw=true "GitLens in use")

6. Since we are working with Git, let's go ahead and see how to work with basic source control in a codespace. First, create a new file. Click on the Explorer icon in the activity bar (#1 in the figure below), then click on the "extra" directory in the explorer so the file will go in the right path (#2), then click on the "New File" icon (#3), and, in the new empty row that pops up, enter the file name (#4). You can name the file whatever you want.

![Adding a new file](./images/spaces26.png?raw=true "Adding a new file")

7. Enter some simple text in the file in the editor tab for it. Then, stage it by clicking on the Source Control icon (#1 in figure below) and then click on the "+" sign (#2) in the 'Changes' area or on the row for the file itself.

![Staging a new file](./images/spaces27.png?raw=true "Staging a new file")  

8. Now you can commit and push the file. In the Source Control view, click on the down area of the green "Commit" button or right click and select the "Commit & Push" option.

![Committing a new file](./images/spaces28.png?raw=true "Committing a new file")  
   
9. At this point, the codespace will present a new tab for you to enter a commit message. The tab will be named "COMMIT_EDITMSG".  Just type in a commit message, then click on the "x" for that tab to save and close the file. This should complete the operation of adding the file into your repository.

![Committing a new file](./images/spaces29.png?raw=true "Committing a new file") 
![Committing a new file](./images/spaces30.png?raw=true "Committing a new file") 

10. Let's look at the Git output after this activity. Bring up the Command Palette by hitting F1 again and type in 'Show Git Output'. Select the option from the list and then switch to the 'OUTPUT' tab in the same section as 'TERMINAL'.

![Rebuilding container](./images/spaces34.png?raw=true "Rebuilding container")    

<p align="center">
**[END OF LAB]**
</p>
  

**Lab 3 - Creating Dev Containers**

**Purpose: In this lab, we’ll see how to create and work with a dev container to persist changes across codespaces**  

1. While we customized our codespace in Lab 2, does that mean that we'll have the customizations persisted if we start up another codespace? Let's find out. Go back to a browser tab that's open with the code repository in your GitHub space. We're going to modify an attribute of our new codespace, so click on the green 'Code' button, then the '...' and then the '+ New with options...' selection.
  
![Starting 2nd codespace](./images/spaces34.png?raw=true "Starting 2nd codespace")    

2. At the options screen for the new codebase, change the 'Machine type' to be '4-core'. (You can also change the Region if you want.) Then click on the green button to create the new codespace.

![Changing options for codespace](./images/spaces36.png?raw=true "Changing options for codespace")   

3. Wait for your new codespace to start up. Once it does, notice that it does not have the color scheme that the previous one had. In fact, there are no extensions installed at all. You can verify this by clicking on the 'Extensions' icon in the Activity Bar and noticing that that the 'BROWSER - INSTALLED' row has a count of 0.

![Codespace without customizations](./images/spaces37.png?raw=true "Codespace without customizations")   

4. Next, we'll create a devcontainer.json file to persist our customizations across all future codespaces. Open the Command Palette (F1) and type in 'devcontainer'.  You should see the 'Codespaces: Add Dev Container Configuration Files...." item in the list. Click on that.

![Create dev container config files](./images/spaces38.png?raw=true "Create dev container config files") 

5. We'll just modify our current configuration instead of creating a new configuration. So, select 'Modify your active configuration'.

![Modify active configuration](./images/spaces39.png?raw=true "Modify active configuration")  

6. After this, codespaces will ask for which features you want to include. There are already a number of features that came preinstalled with the base image that our codespace is based off of. Scroll down to the bottom of the features list and you'll see the ones that are preinstalled.

![Preinstalled features](./images/spaces40.png?raw=true "Preinstalled features") 

7. Let's install the feature for 'podman', an alternative for Docker, in this codespace. In the 'Select Features' text box, type 'podman' and then select the option that comes up. Then click on the blue "OK" button. After this, you should see a new 'devcontainer.json' file opened up in an editor tab.

![Installing podman](./images/spaces41.png?raw=true "installing podman") 
![devcontainer file](./images/spaces42.png?raw=true "devcontainer file")

8. Now, let's install our extensions that we had in the previous codespace. But this time, we'll add them to the devcontainer file so they will be there for new codespaces. Click on the 'Extensions' icon in the Activity Bar, then in the search bar, type in 'Winter is Coming'. After that extension shows up, right-click on it and select the option to 'Add to devcontainer.json'.

![Installing theme](./images/spaces43.png?raw=true "installing theme") 

9. Do the same for the GitLens extension to add it to the devcontainer.json file. Afterwards, your .devcontainer.json file should look as shown below.

![Installing theme](./images/spaces44.png?raw=true "installing theme")
![devcontainer file](./images/spaces45.png?raw=true "devcontainer file")

10. Commit your changes back to the project. Select the 'Source Control' icon in the Activity Bar. We'll use a shortcut here. Just type a commit message in the text entry area above the 'Commit' button, such as "Adding devcontainer.json file".

![adding file](./images/spaces46.png?raw=true "adding file")
    
11. Click on the small down arrow (to the right) on the 'Commit' button and select 'Commit & Push'. You'll see a dialog that comes up telling you there are no staged changes and asking if you want to stage and commit. Just accept the default 'Yes' answer.

![Committing file](./images/spaces47.png?raw=true "Committing file")

12. Before we leave this codespace, let's see what it looks like when we have a problem in the codespace. Go up to the devcontainer.json file and remove the ending quote between the colon and the left bracket of the line that has '"extensions": [' so that it is now '"extensions: ['.  Then switch to the 'PROBLEMS' tab and note the issues reported.
    
![Introducing problem](./images/spaces48.png?raw=true "Introducing problem")   
<p align="center">
**[END OF LAB]**
</p>

13. Add the quote back where it was. The problems in the tab should go away.

14. Now we'll do some management of codespaces through the repository codespace page. In your repository's tab, go to 'https://github.com/<your github userid>/codespaces.

15. On this page you'll see your current codespaces listed. Delete the older one (the one with 2 cores) and Stop the newer one, the one with 4 cores).

![Deleting codespace](./images/spaces50.png?raw=true "Deleting codespace") 
![Stopping codespace](./images/spaces51.png?raw=true "Stopping codespace") 

**Lab 4 - Templates and Ports**

**Purpose: In this lab, we’ll see how to create a codespace from a template and also work with ports.** 

1. Go to the URL at https://github.com/codespaces. Notice your codespaces are listed here. We're going to create a new codespace from a template. Click on the 'See all' link at the top right to see all templates.

![Codespaces page](./images/spaces52.png?raw=true "Codespaces page") 

2. We're going to work with a simple web app built using Flask. In the set of templates, select the one for Flask at the lower left. Click on the name 'Flask' to open it up.

![Template select](./images/spaces53.png?raw=true "Template select") 

3. With the code repo open, take a look at the devcontainer.json file at https://github.com/github/codespaces-flask/blob/main/.devcontainer/devcontainer.json . See if you can understand how it works.

![devcontainer.json file](./images/spaces54.png?raw=true "devcontainer.json file") 

4. Now, go back to the 'Code' tab and click the 'Use this template' green button and select the option to 'Open in a codespace'.

![Open in a codespace](./images/spaces55.png?raw=true "Open in a codespace") 

5. This will start up a new temporary codespace based on the repository. Give it a few minutes to startup and you should see the flask application startup and run in a simple browser tab like the figure below.

![New codespace](./images/spaces56.png?raw=true "New codespace") 

6. Click on the 'PORTS' tab and you'll see two ports forwarded. We're going to redo the port forwarding, so select the port that starts with 'Application (5000', right-click and select 'Stop Forwarding Port'.  Also click on the 'x' in the 'Simple Browser' to close that tab.

![New codespace](./images/spaces58.png?raw=true "New codespace") 

7. Make a simple change to the 'GitHub Codespaces <heart> Flask' line in the 'index.html' file. In the example below, I changed it to add my name and changed some other wording. You can optionally commit the change if you want to keep it for when we publish the repo.

![Modify index.html](./images/spaces60.png?raw=true "Modify index.html") 

8. Next, go to the 'PORTS' tab again. Click on the blue 'Add Port' button and in the text entry field, enter 5000. Hit Enter and you should see the port being forwarded again.

![Restarting port](./images/spaces61.png?raw=true "Restarting port") 
![Restarting port](./images/spaces62.png?raw=true "Restarting port") 
![Restarting port](./images/spaces63.png?raw=true "Restarting port") 

9. Hover over the 'Forwarded Address' column of the row for port 5000, then click on the icon at the end of the column. This should start the app showing in the simple browser tab again.

![Simple browser](./images/spaces64.png?raw=true "Simple browser") 

10. Hover over the 'Forwarded Address' column of the row for port 5000, then click on the middle icon that looks like a globe. This should start the app running in a different browser tab.

![Primary browser](./images/spaces65.png?raw=true "Primary browser") 

11. Go back to the codespace and hover over the 'Forwarded Address' column of the row for port 5000, then click on the left icon. 

![Primary browser](./images/spaces66.png?raw=true "Primary browser") 
   
12. Start a private/incognito session in your browser.  Then paste and try to go to the URL that you copied from the codespace. Chances are you'll get stopped and need to login to see the app running.

![Login required](./images/spaces67.png?raw=true "Login required") 

13. Switch back to the codespaces 'PORTS' tab, select the row for port 5000, and right click. Select the 'Port Visibility' option and make it 'Public'.

![Make port public](./images/spaces68.png?raw=true "Make port public") 

14. Now, repeat steps 11 and 12 to copy the address and paste it into the/a private browser session. This time you should not be prompted to log in and should be able to see the app.

15. Finally, let's publish a copy of our codespace to GitHub to persist it. At the very bottom of the codespace window will be a small icon that looks like an arrow pointing up to a cloud. If you hover over it, will say "codespaces-flask (Git) - Publish to GitHub". Click on that. You will then be prompted in the Command Palette to choose a public or private repo. Choose whichever you want. After that it will upload the files and create the new repo.

![Publish codespace](./images/spaces69.png?raw=true "Publish codespace") 

16. After this, you'll see a popup that says the codespace was published and you can go to the new repo if you want. You can click on it and see your new repo created from the publish.

![Publish codespace](./images/spaces71.png?raw=true "Publish codespace") 

**Lab 5 - Live sharing and collaboration**

**Purpose: In this lab, we’ll see how to share a codespace and collaborate with it.** 

1. In the codespace you were just working in (or one that you startup from the published repo, search for the `Live Share` extension and install it.

![Find and install Live Share extension](./images/spaces72.png?raw=true "Find and install Live Share extension")

2. Click on the `Live Share` icon/link at the bottom of the codespace window.

![Live Share click](./images/spaces73.png?raw=true "Live Share click") 

3. After you click on this, the codespace will copy a sharing link to your clipboard for the codespace.

![Live Share link](./images/spaces74.png?raw=true "Live Share link") 

4. This can be sent in email or any kind of messaging to someone. For now, just paste it into another browser session and it will try to open the app in a web version of Visual Studio Code. You'll see a dialog asking to `Open Visual Studio Code 2.app`. Just click on that button.

![Open VS Code app](./images/spaces75.png?raw=true "Open VS Code app") 

5. Next will be a dialog to `Allow 'Live Share' extension to open this URI?`. Click on `Open`.

![Open extension](./images/spaces76.png?raw=true "Open extension")   

6. On the dialog for signing in with VS Live Share, you can just click `Continue as anonymous`.

![Continue as anonymous](./images/spaces77.png?raw=true "Continue as anonymous")   

7. You can continue as `Guest User` or pick a different name if you want.

![Guest User](./images/spaces78.png?raw=true "Guest User")   

8. After this, you'll see a dialog indicating its waiting for host approval in the new session. Go back to your codespace and click on the `Accept read-write` option.

![Waiting for approval](./images/spaces79.png?raw=true "Waiting for approval") 
![Accept read-write](./images/spaces80.png?raw=true "Accept read-write") 

9. At this point, you should have a new VS Code web session that is connected to your codespace.

![New code session](./images/spaces81.png?raw=true "New code session")    

10. In the new VS Code session, make another simple change to the `index.html` file. In the example, I've added "from other session" to the displayed text. Notice there's also an indicator where the original session is at.

![Change in new session](./images/spaces83.png?raw=true "Change in new session")  

11. Switch back to the original codespace session. You should be able to see the changes in the `index.html` file and if you refresh the browser, you'll see the changes made in the other session. You can also see an indicator of where the Guest User is.

![Change from shared session](./images/spaces84.png?raw=true "Change from shared session")  

<p align="center">
**[END OF LAB]**
</p>

<p align="center">
(c) 2023 Brent Laster and Tech Skills Transformations
</p>
