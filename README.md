# Flask-REST-API-UserEntry
## Steps:-
## Install dependencies:-
```
pip install -r requirements.txt
```
## Database Schema:-
```
CREATE TABLE `emp` (
  `id` int(11) NOT NULL,
  `name` varchar(255) NOT NULL,
  `email` varchar(255) NOT NULL,
  `phone` varchar(16) DEFAULT NULL,
  `address` text DEFAULT NULL
) ENGINE=InnoDB DEFAULT CHARSET=latin1;

ALTER TABLE `emp`
  ADD PRIMARY KEY (`id`);
  
ALTER TABLE `emp`
 MODIFY `id` int(11) NOT NULL AUTO_INCREMENT;
```
## Then run the app:-
```
python3 main.py
```


### 1.View all user data: http://localhost:5000/emp
### 2.View particular user data: http://localhost:5000/emp/{id}
### 3.Create new user data: http://localhost:5000/create
### 4.Update a user data: http://localhost:5000/update
### 5.Delete particular user data: http://localhost:5000/delete/4



