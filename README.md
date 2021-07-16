recipedia
=======
An application that allows users to share cooking recipes, either publicly or among a family or friend group
=======

README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version 2.7.1

* System dependencies
	Devise

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

How to set up:

In your terminal, enter the command:
git clone https://github.com/CaitQuigs/recipedia


rails credentials:edit to create credentials
Enter following information in credentials:
Development database username and password
dev_database_username: <your postgres user name>
dev_database_password: <your postgres password>
dev_database_port: 5432 (should be the port number your postgres server is running on.  Mine is not, so I added it to credentials. You can also remove the credentials call in config/database.yml and skip this step.)
devise_sender_email: <email you want to send devise notifications from>

Save your master key (in master.key) to your password manager. If you lose this key, you will not be able to edit your credentials and you will have to recreate the credentials and re-enter all of them.

Make sure your postgres server is running. Then run:
rails db:create

