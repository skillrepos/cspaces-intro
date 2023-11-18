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

6. After this, codespaces will ask for which features you want to include. There
 
<p align="center">
**[END OF LAB]**
</p>

**Lab 6 – Working with persistent storage – Kubernetes Persistent Volumes and Persistent Volume Claims**
**Purpose: In this lab, we’ll see how to connect pods with external storage resources via persistent volumes and persistent volume claims.**

1.	While we can modify the containers in pods running in the Kubernetes namespaces, we need to be able to persist data outside of them.  This is because we don’t want the data to go away when something happens to the pod.   Let’s take a quick look at how volatile data is when just stored in the pod.

2.	Start up another session of our application running with the following command:

```
kubectl port-forward -n roar svc/roar-web 8089 &
```

3. In the popup that results about "Your applicaton running on port 8089 is available", click on **Open in Browser**.

![Port pop-up](./images/cazclass9.png?raw=true "Port pop-up")

4. In the resulting tab, add **/roar/** (be sure to include the trailing slash) and you should see the running app.

![Running app](./images/cazclass10.png?raw=true "Running app")


5.	There is a very simple script in our roar-k8s directory that we can run to insert a record into the database in our mysql pod.  If you want, you can  take a look at the file update-db.sh to see what it’s doing. Run it, refresh the browser, and see if the additional record shows up.  (Make sure to pass in the namespace – “roar” and don’t forget to refresh the browser afterwards.)  You can ignore the warnings.

```
./update-db.sh <namespace> (such as ./update-db.sh roar)
```

6.	Refresh the browser and you should see a record for “Woody Woodpecker” in the table. Now, what happens if we delete the mysql pod and let Kubernetes recreate it?   

```
k delete pod -l app=roar-db
```

7.	After a moment, a new mysql pod will be started up. When that happens, refresh the browser and notice that the record we added for “Woody Woodpecker” is no longer there.  It disappeared when the pod went away.  

8.	This happened because the data was all contained within the pod’s filesystem. In order to make this work better, we need to define a persistent volume (PV) and persistent volume claim (PVC) for the deployment to use/mount that is outside of the pod.   As with other objects in Kubernetes, we first define the yaml that defines the PV and PVC.  The file [**roar-k8s/storage.yaml**](./roar-k8s/storage.yaml) defines these for us.  Take a look at it now. 

9.	Now create the objects specified here. After this runs, you should see notices that the persistent volume and claim were created.

```
k apply -f storage.yaml
```

10.	Now that we have the storage objects instantiated in the namespace, we need to update our spec to use the values from it.  In the file the change would be to add the lines in bold in the container’s spec area (**you do not need to make changes for this step**):

```
         spec:
           containers:
           - name: mysql
       …
  - name: MYSQL_USER
    valueFrom:
      configMapKeyRef:
        name: mysql-configmap
        key: mysql.user
volumeMounts:
- mountPath: /var/lib/mysql
  name: mysql-pv-claim
        volumes:
        - name: mysql-pv-claim
          persistentVolumeClaim:
            claimName: mysql-pv-claim
```

11.  In the current directory, there’s already a *roar-complete.yaml.pv* file with the changes in it for accessing the secret and the configmap.   Diff the two files with the code diff tool to see the differences.

```
code -d roar-complete.yaml.pv roar-complete.yaml
```

12.  Now we’ll update our roar-complete.yaml file with the needed changes. To save trying to get the yaml all correct in a regular editor, we’ll just use the diff tool’s merging ability. In the diff window, between the two files, click the arrow that points right to replace the code in our roar-complete.yaml file with the new code from the roar-complete.yaml.pv file.  (In the figure below, this is the arrow that is circled and labelled "1".) After that, the files should be identical and you can close the diff window (circled "2" in the figure below).

![Diff and merge in code](./images/k8sdev9.png?raw=true "Diffing and merging for storage")

13.	 Apply the new version of the yaml file to make sure it is syntactically correct.

```
k apply -f roar-complete.yaml
```

14.	 Add the extra record again into the database. (Note you may have to try this a couple of times as it will take a bit for the pod to start up again.)

```
./update-db.sh <namespace>
```

 (such as ./update-db.sh roar)

15.	 Refresh the browser to force data to be written out the disk location.

16.	Repeat the step to kill off the current mysql pod.

```
k delete pod -l app=roar-db
```
    
17.	After it is recreated,  refresh the screen and notice that the new record is still there!

18.	To save on system resources, delete the *roar* namespace.

```
k delete ns roar
```

<p align="center">
**[END OF LAB]**
</p>

**Lab 7 – Working with Helm**
**Purpose: In this lab, we’ll start to get familiar with Helm – an orchestration engine for Kubernetes.**

1. Switch to the caz-class-v2 subdirectory (if not there) and use the tree command to look at the structure.

```
cd  /workspaces/caz-class-v2
tree roar-helm
```
![Helm tree structure](./images/cazclass14.png?raw=true "Helm tree structure")

2. Let’s look at how things map from values to templates to instantiated objects.
Take a look at the template for the roar-web service and then use the template
command to see how the rendered template (with values filled in) looks.

```
cat roar-helm/charts/roar-web/templates/service.yaml
helm template roar-helm/charts/roar-web -s templates/service.yaml
```

3. Finally, let’s look at the values.yaml file for the roar-web charts.

```
cat roar-helm/charts/roar-web/values.yaml
```

4. Next, let’s deploy the full set of charts. First, create the namespace and set the default context to it. (Every other command will be relative to this
context/namespace).

```
k create ns roar2
k config set-context minikube --namespace roar2
helm install roar2 roar-helm
```

5. Get a list of the existing helm deployments and then the status of our current one with the commands below.

```   
helm list
helm status roar2
```

6. We want to look at our app running from the helm deployment. Do a port forward as before. This will start the app running in a browswer as before.

```
k port-forward svc/roar-web 8089 &k port-forward svc/roar-web 8089 &
```

7. You can click on the dialog that pops up to open the app. To see the actual application, add **/roar/** to the end of the URL in the new tab. Don't forget the trailing slash!

8. You will probably notice that while you have the web interface up, there is no data in the table. We’ll fix this next.

![empty app](./images/cazclass15.png?raw=true "App with no data")

9. The problem with our Helm deployment is that the name of the service for the database pod is different than what the web pod expects.  You can see where the name gets set in the “roar-db.name” function in the _helpers template. Select the file  [**roar-helm/charts/roar-db/templates/_helpers.tpl**](./roar-helm/charts/roar-db/templates/_helpers.tpl) to open it.

10. You don’t have to understand all of this, but notice that there are lines in there that mention **default .Chart.Name .Values.nameOverride**
We can interpret this line to say that the default value is Chart.Name, but we also can have an override specified via a “nameOverride” field.

11. Let’s add a nameOverride setting to our values file for the database service chart. Open the file [**roar-helm/charts/roar-db/values.yaml**](./roar-helm/charts/roar-db/values.yaml) and then add the line in bold after the initial comments (or anywhere that is not indented). NOTE that there IS A SPACE between "nameOverride:" and "mysql".

```
# Default values for roar-db-chart.
# This is a YAML-formatted file.
# Declare variables to be passed into your templates.
```
**nameOverride: mysql**
```
replicaCount: 1
```
![updated file](./images/cazclass17.png?raw=true "updated file")

12. Since the format of the value was **.Values.nameOverride**, that indicates that it should be set at the top level of the chart. (If it were something like
.Values.service.nameOverride, that would indicate it should be set in the “service” section of the chart.)

13. Now, that the file has been changed, we’ll do a helm upgrade to get our changes in for the service name. (You’ll need to be in the caz-class-v2
directory.) Run the upgrade. Then check the overall status of the helm release with the helm status command until it shows that things are ready.

```
helm upgrade --recreate-pods roar2 roar-helm
helm status roar2
```

14. You will probably need to redo the port forward command again since we are recreating the pods.

```
k port-forward svc/roar-web 8089 &k port-forward svc/roar-web 8089 &
```

15. Open the app in the browser tab, add the **/roar/** on the end of the URL and you should see the data showing up in the app.
   
16. You can also see the list of helm releases with the command below.

```
helm history roar2
```

17. To save space remove the roar2 namespace.

```
k delete ns roar2
```

<p align="center">
**[END OF LAB]**
</p>

**Lab 8 - Monitoring**

**Purpose:  This lab will introduce you to a few of the ways we can monitor what is happening in our Kubernetes cluster and objects.**

**NOTE: If you run into any issues where the system seems to be hanging and not responding, it may be due to a high cpu load from previous labs. You should be able to fix this via the commands below.**

```
minikube stop
minikube start
```

1.	In order to have the pieces setup for this lab, change to the *monitoring* directory, and run the script *setup-monitoring.sh*. This will take a bit to complete.

```

cd /workspaces/caz-class-v2/monitoring

./setup-monitoring.sh

```

   
2.	First, let’s look at the built-in Kubernetes dashboard. You  can use a simple port-forward to access but then we will need to make one tweak for the port. First do the port forward.

```
k port-forward -n kubernetes-dashboard svc/kubernetes-dashboard :443 &
```

3.	If you look at this in the browser, it will have an error. To fix this, go to the PORTS tab, right-click on the line with "kubernetes-dashboard" in it, click "Change Port Protocol" from the popup menu and then select "HTTPS" from the options. Refresh the browser and you should be able to see the application.

![changing port protocol](./images/k8sdev20.png?raw=true "Changing the Port Protocol")

4.	In the browser, you'll see a login screen.  We'll use the token option to get in.  Switch back to the TERMINAL tab and run the command below and then copy the output.

```
k -n kubernetes-dashboard create token admin-user
```

5.	At the login screen, select "Token" as the access method, and paste the token you got from the step above.

![logging in to the dashboard](./images/k8sdev22.png?raw=true "Logging in to the dashboard")   
 
6.	The dashboard for our cluster will now show.  You can select "All namespaces" at the top, choose K8s objects on the left, and explore.

![working in the dashboard](./images/k8sdev21.png?raw=true "Working in the dashboard")
 
7.	Now let’s look at some metrics gathering with a tool called Prometheus. First, we will do a port-forward to access the Prometheus UI in our browser.

```
kubectl port-forward -n monitoring svc/monitoring-kube-prometheus-prometheus :9090 &
```

8.	Open this in the browser via the port button. You should see a screen like the one below:

![prometheus opening screen](./images/k8sdev23.png?raw=true "Prometheus opening screen")
 
9.	Prometheus comes with a set of built-in metrics.  Just start typing in the “Expression” box.  For example, let’s look at one called “apiserver_request_total”.  Just start typing that in the Expression box. After you begin typing, you can select it in the list that pops up. After you have got it in the box, click on the blue “Execute” button.

![prometheus metrics entry](./images/k8sdev24.png?raw=true "Prometheus metrics entry") 

10.	Now, scroll down and look at the console output (assuming you have the Table tab selected).

![prometheus console output](./images/k8sdev25.png?raw=true "Prometheus console output")

11.	Next, click on the blue “Graph” link next to “Console” and take a look at the graph of responses.  Note that you can hover over points on the graph to get more details. You can click "Execute" again to refresh.

![prometheus graph view](./images/k8sdev26.png?raw=true "Prometheus graph view")
 
12.	You can also see the metrics being automatically exported for the node. Do a port forward on the node-exporter service and then open via the port as usual.

```

kubectl port-forward -n monitoring svc/monitoring-prometheus-node-exporter 9100 &

```
Click on the **Metrics** link.

![metrics view](./images/cazclass18.png?raw=true "Metrics view")

13.	 Now let’s change the query to show the rate of apiserver total requests over 1 minute intervals.  Go back to the main Prometheus screen.  In the query entry area, change the text to be what is below and then click on the Execute button to see the results in the graph.

```

rate(apiserver_request_total[1m])

```
![prometheus rate query](./images/k8sdev27.png?raw=true "Prometheus rate query")

14.	Finally, let’s take a look at Grafana. First you need to get the default Grafana password. You can get that by running the *./get-grafana-initial-pw.sh* script in the *monitoring* directory.

15.	 Then you can do a port forward for the "monitoring-grafana" service.  

```

k port-forward -n monitoring svc/monitoring-grafana :80  & 

```

16.	Go to the browser tab. Login with username *admin* and the initial password.

![grafana login](./images/k8sdev28.png?raw=true "Grafana login")


17.	  Click on the magnifying glass for "search” (left red circle in figure below). This will provide you with a list of built-in graphs you can click on as demos and explore.

![grafana search](./images/k8sdev29.png?raw=true "Grafana search")  
 
18.	 Click on one of the links to view one of the demo graphs (such as the "Kubernetes / API server" one) shown in the figure below). You can then explore others by discarding/saving this one and going back to the list and selecting others.

![grafana demo graph](./images/k8sdev29.png?raw=true "Grafana demo graph") 

<p align="center">
**[END OF LAB]**
</p>

<p align="center">
(c) 2023 Brent Laster and Tech Skills Transformations
</p>
