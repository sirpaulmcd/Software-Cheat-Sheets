# Virtual Environments?

## What are virtual environments and why should I care?

Virtual Environments are great for large software projects. Virtual environments:

- Ensure projects only have access to the dependencies and packages that they need (good practice).
- Ensure old projects are not broken when packages are updated for use in new projects. 

For example, let's assume a person created a Python 2 project in their base environment. Sometime after, they started work on a project using Python 3. Since these projects share the same environment, the Python 2 package will have been updated to Python 3 causing the older project to break. Virtual environments provide projects with an isolated environment where package versions are exclusive to the project. 

## Python (and R) virtual environments through Anaconda

### Initial setup

Note that you can also use the `virtualenv` package to create/manage Python virtual environments. However, I find that it's easiest to use through the Anaconda Navigator. 

The steps are as follows:

1. Open the Anaconda Navigator
2. Go to the environments tab and select the "Create" button:

![image-20200501134931621](C:\Users\sirpa\AppData\Roaming\Typora\typora-user-images\image-20200501134931621.png)

3. Enter your project name and desired base packages and submit.
4. Congratulations you now have a fresh python virtual environment. You can begin installing your required packages using the pip command or through the Anaconda Navigator. 

### Activating a virtual environment

In order to use a virtual environment, it has to be activated for each unique terminal instance:

- Activate in terminal using `conda activate [Environment Name]`
  - If you're using Windows PowerShell, if the above does not work, use the command `& cmd /k "activate  & powershell"` and try again.

- You may also need to indicate the desired environment in your IDE. For example, in VSCode, this option can be selected on the bottom bar:

![image-20200501141230862](C:\Users\sirpa\AppData\Roaming\Typora\typora-user-images\image-20200501141230862.png)

