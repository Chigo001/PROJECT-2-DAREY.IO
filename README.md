STEP 4: PROJECT 2
WEB STACK IMPLEMENTATION (LEMP STACK)
- Go to your AWS Console and create a new instance and ssh into the instance.

STEP 1
- INSTALLING NGINX WEB SERVER
- To display web pages on our websites, we will need to deploy Nginx. We will use the 'apt' package manager to install this package.
- Update apt for the session 
- Apt install to get Nginx installed
- Enter Y to confirm Nginx installation 
<img width="1440" alt="Screenshot 2022-10-19 at 1 10 19 PM" src="https://user-images.githubusercontent.com/115854902/197346933-2fcf9ace-b04d-4d39-947e-e89feeb27965.png">
- Verify the successful installation of the Nginx 
<img width="1440" alt="Screenshot 2022-10-19 at 1 13 41 PM" src="https://user-images.githubusercontent.com/115854902/197347469-53dee57c-4934-4808-af33-960ee2dfd87d.png">
- Add a rule to EC2 configuration to open TCP port 80
- Use curl command to access Nginx on the Ubuntu shell
<img width="1440" alt="Screenshot 2022-10-19 at 1 44 07 PM" src="https://user-images.githubusercontent.com/115854902/197347653-548ec0ba-56d9-422d-8f09-6d126d89122e.png">
- Copy IP address  and open on a web browser 
<img width="1440" alt="Screenshot 2022-10-19 at 1 46 57 PM" src="https://user-images.githubusercontent.com/115854902/197347802-ebb14c3e-34d4-45f8-b510-912d90ba4009.png">

STEP 2: INSTALLING MySQL 
- Use apt to acquire and install MYSQL
- Confirm installation by typing Y and enter 
 <img width="1440" alt="Screenshot 2022-10-19 at 2 18 19 PM" src="https://user-images.githubusercontent.com/115854902/197348103-be604a61-85a2-4bfe-8fe3-3951a235c19a.png">
- Log into the MYSQL Console

<img width="1440" alt="Screenshot 2022-10-19 at 2 20 46 PM" src="https://user-images.githubusercontent.com/115854902/197348227-25dd09aa-b897-452b-90af-c56ec9635b61.png">
- Run a security script that comes pre-installed with MySQL

<img width="1440" alt="Screenshot 2022-10-19 at 2 35 41 PM" src="https://user-images.githubusercontent.com/115854902/197348529-2c56367d-3645-4285-bd25-948c48bf9c41.png">
-Exit MySQL shell

- Start the interactive script
- Log into MySQL Console again then exit.
<img width="569" alt="Screenshot 2022-10-20 at 1 26 58 PM" src="https://user-images.githubusercontent.com/115854902/197348747-5c5f4a99-d28b-447d-a1eb-d3d082bb6265.png">
<img width="1440" alt="Screenshot 2022-10-19 at 2 35 41 PM" src="https://user-images.githubusercontent.com/115854902/197348900-d4d9e9b3-8b28-4070-9d74-dc65a351d277.png">

STEP 3: INSTALLING PHP
- Install 2 core PHP packages 
<img width="1440" alt="Screenshot 2022-10-20 at 2 04 48 PM" src="https://user-images.githubusercontent.com/115854902/197349120-3bc346f9-e02a-4d40-878f-9080a8bb4a71.png">

<img width="1440" alt="Screenshot 2022-10-20 at 2 05 42 PM" src="https://user-images.githubusercontent.com/115854902/197349141-1061f15c-5715-48a0-8ba5-3a15c7b8109d.png">

STEP 4: CONFIGURING NGINX TO USE PHP PROCESSOR.
- Create root web directory
- Assign ownership of the directory with the user environment variable .
- Open a new configuration file using nano
- paste the barebones configuration in the new blank file, save and close the file.
- Activate your configuration 
- Test your configuration for syntax error
- Disable default Nginx host
- Reload Nginx to apply changes .

<img width="1440" alt="Screenshot 2022-10-21 at 11 15 26 AM" src="https://user-images.githubusercontent.com/115854902/197351284-78a04c2a-e52a-410a-b5d9-010fbc34f91c.png">
- Go to browser and enter public IP address or public DNS name to see text from echo you have entered.

<img width="1440" alt="Screenshot 2022-10-20 at 2 18 47 PM" src="https://user-images.githubusercontent.com/115854902/197351803-d854ac37-7ea6-4aed-8819-f3801e3bb5b8.png">

STEP 5: TESTING PHP WITH NGINX
- Create a file in your  document root
- Paste the valid PHP Code into the new file, save it and proceed.

<img width="1440" alt="Screenshot 2022-10-21 at 11 26 08 AM" src="https://user-images.githubusercontent.com/115854902/197352398-ad757bc1-54ab-4189-8682-3ce575ff06c0.png">

Go to web browser to access this page using your public IP address.

<img width="1440" alt="Screenshot 2022-10-21 at 8 19 53 PM" src="https://user-images.githubusercontent.com/115854902/197352456-182da05a-53fa-4a3c-95fe-d3d2cf8b1943.png">

STEP 6: RETRIEVING DATA FROM MYSQL DATABASE WITH PHP (CONTINUED)
- Connect to the MySQL console using the root account.
- Create a new database and replace the password with a secured password of your own.
- Give the user permission over the example_database then exit

<img width="1440" alt="Screenshot 2022-10-22 at 1 32 16 AM" src="https://user-images.githubusercontent.com/115854902/197352794-28c206c9-011b-4eca-aaba-2d1d93390255.png">
- log into MySQL console again , confirm that you have access to the database
- Create a test table named todo-list
- Insert a few roles content
- Confirm data successfully saved then exit
- Create a php script that will connect to MySQL and query for your content
- Copy content into your todo list then save and close.

<img width="1440" alt="Screenshot 2022-10-22 at 1 52 18 AM" src="https://user-images.githubusercontent.com/115854902/197353084-5813b1e7-cc17-44d8-b5c6-09493c65d7ca.png">


<img width="1440" alt="Screenshot 2022-10-22 at 2 06 19 AM" src="https://user-images.githubusercontent.com/115854902/197353086-72421c12-5bc3-448f-b94a-4458d4151cbc.png">

Access this page in your web browser using your public IP address.

<img width="1440" alt="Screenshot 2022-10-22 at 4 36 21 AM" src="https://user-images.githubusercontent.com/115854902/197353159-93e54342-e839-4449-bc26-d8d2f5395a7a.png">














