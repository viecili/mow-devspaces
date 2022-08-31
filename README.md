# Welcome to the Enterprise Kubernetes Workshop

Today we will be running through a hands on workshop where we will learn and play with some of features of Red Hat OpenShift.
 
## Useful Links

- **Workshop Instructions**
    - on Azure (ARO): https://rh-anz-aro-workshop.github.io/anzaroworkshop/
    - on AWS (ROSA): 
- Set up free GitHub Account if you dont have one already: https://github.com/join

## How to run the Terminal
- Click the menu `Terminal > New Terminal`
- In the drop down list, select `jumpbox`
    - a terminal pane should open at the bottom of the screen
- Click on the terminal pane and type `oc whoami` then press `ENTER`
    - you should see your username, e.g. `user1`


## Resources for Exercise 2

Open the Terminal (see above), and run: 

```zsh
wget https://raw.githubusercontent.com/RH-ANZ-Workshops/anzworkshop/main/yaml/ostoy-fe-deployment.yaml
wget https://raw.githubusercontent.com/RH-ANZ-Workshops/anzworkshop/main/yaml/ostoy-microservice-deployment.yaml
```

**OR** 
- Click the menu `Terminal > Run Task...`
- From the drop down, select `get-ostoy-fe` to download the `ostoy-fe-deployment.yaml` file. 

Repeat the first step above and select `get-ostoy-microservice` to download the `ostoy-microservice-deployment.yaml` file.



## Feedback Survey link: https://red.ht/FeedbackARO

