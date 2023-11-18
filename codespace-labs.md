# Understanding and using GitHub Codespaces
## Session labs for codespace only
## Revision 1.0 - 11/16/23

**NOTE: To copy and paste in the codespace, you may need to use keyboard commands - CTRL-C and CTRL-V.**

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

14. 

15. 
<p align="center">
**[END OF LAB]**
</p>

<p align="center">
(c) 2023 Brent Laster and Tech Skills Transformations
</p>
