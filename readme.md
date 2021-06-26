# Jenkins Cheat sheet for Ubuntu & macOs

> Jenkins is an Open-Source project written in JAVA that runs on Windows, macOS and Other Unix like Opareting system.

> Jenkins was Originally developed by SUN Microsystem in 2004 under the name Hudson. 

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


[MASTER-ACADEMY](https://master.com.bd/)
