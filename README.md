# orchestraDocker
 ## To Use:
 1. Fork this repository. 
 2. Install Docker on your computer (https://www.docker.com/get-started) and create a docker ID / sign-in
    * After installation run the following commands in terminal (to verify Docker installed properly):
      * ```docker version```
      * ```docker run hello-world```
 3. Install Visual Studio Code (https://code.visualstudio.com/download) and 
    * Install the following VS Code extentions (from within the app, left-hand menu square grid style icon):
      * Docker (by Microsoft)
      * Remove Development (by Microsoft)
      * C/C++ (by Microsoft)
4. Clone forked repository to computer.
5. Download Orchestra SDK Linux C++ tgz file from collaborate.mr.gehealthcare.com (login required) and put into ./orchestra directory (https://collaborate.mr.gehealthcare.com/servlet/JiveServlet/downloadBody/1634-102-2-2289/orchestra-sdk-1.8-1.x86_64.tgz)
6. Open cloned repository in Visual Studio Code.
7. Right click on Dockerfile (in VS file explorer) and click "Build Image" Hit enter to accept label (orchestraDocker:latest is default, but it doesn't matter)
8. Click Remote-Development Button in lower left hand of screen bottom toolbar. Select "Reopen in Container." Wait for installation (first time takes longer)
9. Terminal > New Terminal
   * ```pwd``` Will show your working directory in the docker container. Think of this as the "mounted" location of your local project folder.
   * ```cd project```
   * ```cmake ./``` (If you get an error, just do it one more time. Usually it works the 2nd time)
   * ```make```
   * ```cd ./BuildOutputs/Release/bin```
   * ```./demo```
   * ```cd /workspaces/orchestraDocker/project```
   * Create a new git branch with a custom branchName to describe your project. ```git branch branchName```
   * ```git checkout branchName```
