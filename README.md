# TcUnit_LibraryTemplate
A template library and instructions on how to add the files to have the project added as a template inside the TwinCAT 3.

To create custom project template, follow these steps.

1. Download the files in this repo
2. Go to ```C:\TwinCAT\3.1\Components\Plc\PlcTemplates\1.0.0.0```
3. Copy the files in this location
4. The ```PlcTemplates.vsdir``` file will be edited. Opt to replace or edit the file manually. Add the following line
  - ```Tests template.plcproj|0|Library with unit tests template|3|Creates a project template for library creation and testing using the TcUnit Framework.|0|0|0|0```
5. If you had your TwinCAT opened, close it and re-open it.
6. Try to add new PLC project to your solution, you can now select the following template

![image](https://github.com/user-attachments/assets/e7bab93c-c90c-48b5-b6de-dc829983d3fc)
7. A new project with the following structure is created

![image](https://github.com/user-attachments/assets/4a16a5c8-7f55-4662-82e9-7c50ade37793)

Project structure description:
- References
  - Added ```TcUnit``` reference, with latest installed version
  
    ![image](https://github.com/user-attachments/assets/81f39c8b-d590-463a-9551-a1eb28d85bf8)

  -  ```Source``` folder is used to place your source code, the implementation logic.
  -  ```TESTS``` folder will contain all the tests suites required to test the objects from ```SOURCE``` folder.
  -  ```Test suites``` folder contains the implementation of tests. Use ```FB_SUT_Tests``` as a template to create them.



