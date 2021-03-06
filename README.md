# Programming Works Competition

### Brief Introduction

This is a naive online web system for **Programming Works Competition** with `Register`, `Login`, `Information Check(Teams)`, `File Upload` and `Forum` functions provided.

- Register: You can register as `Production Team` or `Creativity Team`, while `Creativity Team` can include **3** members at most and `Production Team` can include **5** at most
- Login: Already registered teams can login this system with the `TeamID` provided at the time of registration, and then you can see the detailed information of your team members and use upload function to submit you entry. Additionally, if any team forgets their password, it's still easy to reset it once the right information of team leader is inputted.
- Teams: By default, this page shows brief information of all teams and their members. If you are logged in, detailed information of your team will show in the third part, with which you can check if the information is correct
- Upload: This part is built with [bootstrap-fileinput](https://github.com/kartik-v/bootstrap-fileinput), and you can upload the entry of your team with **Compressed Package Format** when logged in
- Forum: Anyone can see all the messages currently as well as leaving a message with a nickname

The interface of this project is based on [Bootstrap](http://getbootstrap.com/) Front-end Framework, and it is my first time to use Front-end Framework.

**Note: Preview pictures of this system are stored in [`./assets/pictures/preview`](./assets/pictures/preview)**

### Deployment Tutorial
1. Use `initDB.sql` to create the database with necessary tables, change the default database name `competition` if it's necessary
2. If you use the Full Version instead of Default Version(See [Releases](https://github.com/KingsleyXie/ProgrammingWorksCompetition/releases)), please remember to remove: `importData.php` **(Especially!)**, `initDB.sql` and `registerformFill.js` to somewhere else that can't be accessed by website visitors, and deploy the files on your server
3. Modify `assets/config.php` with the instructions inside the file, normally they are: 
    - **Database Name**
    - **Username for Project Database**
    - **Password for Project Database**
    - **Upload File Directory**
    - **Backup File Directory**
4. Make sure your server can run PHP files correctly and then you don't need to modify any code
5. Have some test before make it online to run, and replace files in `assets/pictures` with pictures corresponding to your competition
