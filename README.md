# [Admin Dashboard](https://admindashboardfrontend-wa7b.onrender.com)
![Screen Shot 2023-03-11 at 6 57 28 PM](https://user-images.githubusercontent.com/22222231/224519963-a6ac998c-5194-433a-8fc2-07139fc65b5b.png)

Responsive, mobile compatible, full stack Admin Dashboard application with the ability to navigate products, customers, transactions, user location geography, sales, admin management and more.

# Stack
![Mern-1](https://user-images.githubusercontent.com/22222231/224519858-07da5cef-d3d7-4e39-900f-6f2baff9b38c.jpeg)

# DB Architecture
![Screen Shot 2023-03-11 at 6 49 09 PM](https://user-images.githubusercontent.com/22222231/224519897-9f95320a-56c8-4e44-8e9e-fe7198ed3a97.png)

# Admin Viewability
Browse products - each product containing a description, rating, and price.

![Screen Shot 2023-03-11 at 6 58 48 PM](https://user-images.githubusercontent.com/22222231/224520036-90462d4d-bf5b-421b-9d51-7172026dc264.png)

View Customers - each customer is represented as a user with an ID, name, email, phone number, etc.

![Screen Shot 2023-03-11 at 7 00 16 PM](https://user-images.githubusercontent.com/22222231/224520062-756280c3-4337-4532-a659-f67463b3d3ec.png)

Recent Transactions - Each transaction has a unique ID and a corresponding User that generated that transaction. Admins can view these transactions in order to troubleshoot business processes. 

![Screen Shot 2023-03-11 at 7 01 01 PM](https://user-images.githubusercontent.com/22222231/224520071-8e1e4d8e-3004-4b14-bede-4e1f3fefdacd.png)

View Map of User Geography - User data is quried from our MongoDB and a request is sent to [Nivo Rocks](https://nivo.rocks/choropleth) in order to get the geography map data (Choropleth chart). 

![Screen Shot 2023-03-11 at 7 01 29 PM](https://user-images.githubusercontent.com/22222231/224520089-3930c04a-3290-4412-b1c1-26d759deeb06.png)

Sales Overview - Graph of the sales overview is included for display. Admins can view this chart and take action depending on the trajectory.

![Screen Shot 2023-03-11 at 7 02 05 PM](https://user-images.githubusercontent.com/22222231/224520098-a8871b00-1a19-4333-93af-b035d9577478.png)

Daily Sales

![Screen Shot 2023-03-11 at 7 02 24 PM](https://user-images.githubusercontent.com/22222231/224520108-b33d0954-4935-45f7-84b7-6dc94303983e.png)

Monthly Sales

![Screen Shot 2023-03-11 at 7 02 41 PM](https://user-images.githubusercontent.com/22222231/224520115-142997be-7587-4f68-a7f5-41cae0890915.png)

Sales Breakdown

![Screen Shot 2023-03-11 at 7 03 02 PM](https://user-images.githubusercontent.com/22222231/224520128-16065c48-2ef2-4078-8427-2a31d406e935.png)

Admin List - List of the users allowed as admins. 

![Screen Shot 2023-03-11 at 7 03 23 PM](https://user-images.githubusercontent.com/22222231/224520141-636cbbb0-fe00-455b-baf7-e6906f564574.png)

View Performance - Performance of users can be viewed if you're an admin.

![Screen Shot 2023-03-11 at 7 03 31 PM](https://user-images.githubusercontent.com/22222231/224520149-b0e18890-b6ff-434f-92c2-7948309f67fa.png)

Light Mode - toggle between dark mode and light mode depending on preference.

![Screen Shot 2023-03-11 at 7 04 15 PM](https://user-images.githubusercontent.com/22222231/224520162-7d749b04-270f-45b2-85a6-3fc22ac18e68.png)



# Deployment
![Screen Shot 2023-03-11 at 6 49 38 PM](https://user-images.githubusercontent.com/22222231/224519900-e0abc13d-b749-40a8-be46-35127c831b9c.png)

Deployment architecture is as follows. Our data is stored in our mongoDB database, which communicates with our server. This server and client are hosted on render. When you visit the deployed site, you're really just visiting the deployed client site. However, this communicates with our backend (also hosted on render). Render will communicate with github for us and refresh the deployment anytime a change is made to the main branch. Note: Environemnt variables and node modules are **not** pushed to github (gitignore). Env variables are set up on render.
