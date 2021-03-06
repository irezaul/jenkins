# Jenkins Cheat sheet for Ubuntu & macOs

> Jenkins is an Open-Source project written in JAVA that runs on Windows, macOS and Other Unix like Opareting system.

> Jenkins was Originally developed by SUN Microsystem in 2004 under the name Hudson..

> It's free! strong Community Supported and lots of Plugins are available and might be your first choice tool for CI (continuous integration).

> Jenkins automade the entire Software Development life-cycle.

> Whenever developer's write code, we intrigate all that code of all developers at that point of time and we build, test & deploy/deliver to the client. (this process are called CI/CD).

> Jenkins help us to achive this. beacuse of CI nows bugs(error) will be reported fast and get rectified fast. so the entire software development happens fast.


# install to macOS
``` bash
brew install java

```
![java install](https://user-images.githubusercontent.com/77927449/123520597-39bc0900-d6d3-11eb-9376-3b7dcda9effd.png)

#### 2nd step
``` python
brew install jenkins-lts
```
![Jenkins install](https://user-images.githubusercontent.com/77927449/123520757-13e33400-d6d4-11eb-8f84-d9ec84dc8c1c.png)

#### 3rd step

```
brew services start jenkins-lts   
brew services stop jenkins-lts
brew services status jenkins-lts   
```

# Install to Ubuntu

#### 1st step
``` bash 
sudo apt-get update
```
####  added the repository key to the system:
``` bash
wget -q -O - https://pkg.jenkins.io/debian-stable/jenkins.io.key | sudo apt-key add -
```
#### added debian package repository address :
``` bash
sudo sh -c 'echo deb http://pkg.jenkins.io/debian-stable binary/ > /etc/apt/sources.list.d/jenkins.list'
```
#### update apt :
```bash
sudo apt update
```
#### Finally install Jenkins -
```bash
sudo apt install jenkins
```

#### Now start, status & stop alos working -
``` bash
sudo systemctl start jenkins
sudo systemctl status jenkins
sudo systemctl stop jenkins
```

If you need any question & need to added somthing please info me....
[rezaulkarim](fb.com/mtmartbd)

## How to added a agent -
##### Go Jenkins Dashboard click to `Nodes` then click to `New Nodes`

![Jenkins nodes](https://user-images.githubusercontent.com/77927449/128058427-d86b9ce0-6e8f-4141-b2dc-5ebaa8926e6e.png)

##### click on add node & next show this screen & copy the `agent.jar` link..

![node_link](https://user-images.githubusercontent.com/77927449/128058940-cecb3668-46e6-4f78-87fe-ae3bbc5fe18c.png)

![agent jar_](https://user-images.githubusercontent.com/77927449/128059185-9b59b625-90de-402c-a7ac-32d4e0def20f.png)

#### now go to Host Machine & download `Agent.jar`
##### go to the home directory & download it by command-

```bash
wget http://192.168.1.11:8080/jnlpJars/agent.jar
```
![agent_file](https://user-images.githubusercontent.com/77927449/128060376-4162abf4-a471-4e9d-98f7-29d90c22a3c0.jpeg)

#### then run the command which jenkins give to you when added node.

![node_link](https://user-images.githubusercontent.com/77927449/128058940-cecb3668-46e6-4f78-87fe-ae3bbc5fe18c.png)

### Example-
```bash
java -jar agent.jar -jnlpUrl http://192.168.1.11:8080/computer/agent1/jenkins-agent.jnlp -secret a7c38d66f03fe6be49aa7484b4a1f5acbd662db3acc92bfc51abc813f9e0bd3c -workDir "/home/"
```
#### Now your node ready -

![node-added](https://user-images.githubusercontent.com/77927449/128060468-75f3513c-d440-4845-b637-83280bc75110.jpeg)





[MASTER-ACADEMY](https://master.com.bd/) 
join here [codingbootcamp](fb.com/groups/codingbootcampbd)




