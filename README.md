# go-env-ways

Why should we use the environment variable?
Suppose you have an application with many features and each feature need to access the Database. You configured all the DB information like `DBURL`, `DBNAME`, `USERNAME` and `PASSWORD` in each feature.

There are a few major disadvantages to this approach, there can be many.

Security Issue:

You’re entering all the information in the code. Now, all the unauthorized person also have access to the DB.
If you’re using code versioning tool like git then the details of your DB will go public once you push the code.

Code Management:

If you are changing a single variable then you have to change in all the features. There is a high possibility that you’ll miss one or two. 😌 been there
You can categorize the environment variables like PROD, DEV, or TEST. Just prefix the variable with the environment.
