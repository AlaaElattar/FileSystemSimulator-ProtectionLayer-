# File System Simulator (Protection Layer)
Build up a protection layer over the simple file system, the protection module will be responsible of the following activities :
* **1- Creating Users**
* **2- Assign capabilities to users : Each folder will have two capabilities Create/Delete**

### After running the application a default user will be logged in to the system this user is called “admin” with the password “admin”, the commands in the table below will be added to the list of the commands : <br/>

**1. TellUser** <br/>
 * *This command will display the name of the current logged in user.* 


**2. CUser ahmed pass123** <br/>
 * *This command used to create user named “ahmed” with the password “pass123”.* 
   * Comments : <br />
      1- only the admin can use such command. <br/>
      2- No user with the same name already created. </br>
      
**3. Grant ahmed root/Folder1 10** <br/>
 * *This command is used to grant the user “ahmed” Create and Delete Capabilities on the folder “root/older1”.* 
   * Comments : <br />
      1- 1- only the admin can use such command. <br/>
      2- This command is used for folders only. </br>
    * Pre-requests : <br/>
      1- The path already exists. <br/>
      2- The user already exists. <br/>
      
**4. Login ahmed pass123** <br/>
 * *After this command the current logged in user will be “ahmed” instead of admin.* <br/> 
 * *All assignment 3 commands now must be checked before its execution with the user “ahmed” capabilities.* <br/> 
 * *This command is used to change the current logged in user with the user “ahmed”.*
    * Pre-requests : <br/>
      1- The user already exists. <br/>
      2- The password is correct. <br/>
      

