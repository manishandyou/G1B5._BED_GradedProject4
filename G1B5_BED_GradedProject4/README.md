# G1B5._BED_GradedProject4
Login credentials

For Admin -> all access
1) username: admin
   password: admin

For User -> access to only GET methods
2) username: user
   password: user
   
  
   mysql queries used:
   -- create database
    create database employeeDatabase;
    use employeeDatabase;
   
   
  -- insert data into employees table 
INSERT INTO employees (id, email, first_name, last_name) 
VALUES (1, 'pooja@gmail.com','pooja','chavali'),
	   (2, 'sneha@gmail.com','sneha','sri'),
       (3, 'john@gmail.com','john','louis'),
       (4, 'nikhil@gmail.com','nikhil','reddy'),
       (5, 'aparna@gmail.com','aparna','sharma'),
       (6, 'kiran@gmail.com','kiran','jajula');
       
 
   -- insert data into role table
INSERT INTO role (id, name)
VALUES (1, 'ADMIN'),
	   (2, 'USER');

    -- insert data into user table
	   
INSERT INTO user (id, password, username)
VALUES (1, '$2a$08$Y09I.9niV5KM8Y/NhZ.pb.QD03JityCaq/AIe5R01qbnvKrsXpUMW', 'admin' ),
	   (2, '$2a$08$3MUTJa2KaWEjsj8Ks6aA/uzbCig4crD5MwLSMY4ezdwERKxRWPxKK', 'user');
	   
	   --
	   --password for admin --> admin
	   --password for user  -->user
 	   --
 	   
    -- insert data into users_roles table   
INSERT INTO users_roles(user_id, role_id)
VALUES (1, 1),
	   (2, 2);  
