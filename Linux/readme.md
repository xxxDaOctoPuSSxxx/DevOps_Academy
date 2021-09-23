# Linux Lessons<br/>
## Task 1:<br/>
### Part1
   - Login to system as root **sudo su**;
   - Change password **passwd** yuo must be **SU** take constrution **passwd username**;
   - Determine users **whoiam, who, w**;
   - Linux **HELP** system **man** use to take manual **man** _programname_.<br/>
   
   
### Part2
   - **tree** _command_ printed files in tree visualization;
   - **file** _command_ with different keys use to determine type of file;
   - **cd~/** comeback from any directory to **/home/**
   

## Task 2 :<br/>
 1. If use **cat/etc/passwd** command show information about all users registred in filesystem.<br/>
-  If use **cat/etc/group** command show information about all groupsregistred in filesystem.<br/>
-  **pseudo-users** Users of these names are not registered in the system and are only needed to confirm ownership of the processes. It has, **id** from **1** to **499** sometime **999** <br/>

2. **UID - User identifier** values in the range 0 to 99 should be **statically allocated** by the system, and shall not be created by applications, while **UIDs** from **100 to 499** should be **reserved** for dynamic allocation by system administrators and post install scripts.  <br/>
 To find **UID** use the command **id** **cat/etc/passwd** 
3. **GID - group identifier** To find **GID** use the command **id** **cat/etc/passwd**
4. To determine belonging of user to the specific group need to use the _command_ **groups username**
5. **useradd** are the command for adding a user to the system. <b/>
Basic parameters required to create a user are **username, password, /home/ shell** <b/>
6. To change the name (account name) of an existing user use the _command_ **sudo usermod -l new_username old_username**

7. The **skel_dir** is **template** for a **home** directory of _new user_.
8. To **remove** a user from the system (including his mailbox) use **userdel [-r] username**
9. The _commands_ and _keys_ should be used to lock and unlock a user account is **usermod -f** **usermod -e**
10. To remove a user's password and provide him with a password-free login for subsequent password use the _command_ **passwd -e username**
11. To display the extended format of information about the directoryuse the _command_ **ls -l**
12. The access rights exist at _file_ or _directory_ has tree parameers **owner, group, others**
13. The sequence of defining the relationship between the file and the user is **owner**
14. The _command_ are used to change the owner of a file (directory), is **chown ugo+-rwx, or numeric**
15. An example of octal representation of access rights is numeric **chmod 777** all rights are aprouwed for all ugo
16. **Sticky Bit** is mainly used on folders in order to avoid deletion of a folder and it’s content by other users though they having write permissions on the folder contents.
17. The file attributes should be present in the command script looks like combination rwxrwxrwx

