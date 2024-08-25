# Database Wars: Comparing Firebase, MongoDB, and SQL for App Development

Hey reader 👋,

I chose this topic because of my 2nd greatest teacher who taught Database and Management Systems in my 1st semester… LOL 😅

Just for educational purposes: 1st position is always held by **#Prashant OP sir** (only IIITL students feel my pain 🥲🥲).

Okay, enough about them!

From that class, I got super curious about how big websites and apps are storing and managing all this massive data, and like... how they do it for free?? And even when we use it, they give us data in just a few seconds (or milliseconds if we're lucky)!

Then I found out about these 3 big databases everyone keeps talking about. So I thought to share them with you:

## MongoDB 🍃

![MongoDB Logo](assets/mongo.jpeg)

MongoDB is the no-SQL wild child of the database world. Instead of organizing data into rows and tables like SQL, MongoDB stores data in flexible documents.

### Pros:
- **Schema Flexibility FTW:** Unlike SQL, MongoDB doesn’t care if your data doesn’t fit neatly into predefined rows and columns. Got a random new field to add? Just throw it in! MongoDB’s like, "Cool, I got this."
- **Scalability Like a Pro:** MongoDB scales horizontally with ease. You can spread your database across multiple servers without breaking a sweat. More users? More servers. No problemo!
- **Great for Unstructured Data:** If your app is collecting unpredictable, messy, unstructured data (like images, files, or, idk, random thoughts), MongoDB’s got you covered.

### Cons:
- **Querying is a Learning Curve:** MongoDB querying isn’t as straightforward as SQL’s, “SELECT * FROM complaints WHERE upvotes > 100.” You’ll need to get cozy with its own query language.
- **Not Always the Best for Complex Relationships:** MongoDB handles data well when it’s loosely connected. But when you need to do a lot of joins (like relating student complaints to admins and guards), MongoDB can feel a bit… messy. Kind of like my code before I debug it. 😅

### Best For:
- **Startups or apps** that deal with unstructured data or need to scale horizontally with ease. Also good for projects where flexibility is key and your data doesn’t fit into neat rows.

---

## SQL Databases (MySQL, PostgreSQL, etc.) 🧑‍💻

![SQL Logo](assets/sql.jpeg)

Ah yes, the OGs of databases—the ones we learn in our textbooks but end up fearing during exams. SQL databases like MySQL and PostgreSQL are the kings of structure and order. They use tables with rows and columns, and they are relational, meaning data is related across multiple tables through primary and foreign keys.

### Pros:

![funny image](assets/sql1.jpg)
- **Relational Powerhouse:** SQL databases shine when your app has data with complex relationships. Need to relate students to complaints, complaints to admins, admins to their favorite cafeteria snack? SQL’s got you covered.
- **ACID Compliance:** No, not the acid you’re thinking of. This stands for Atomicity, Consistency, Isolation, and Durability—basically, SQL databases are super reliable when it comes to data integrity. No funny business.
- **Mature Ecosystem:** SQL has been around for a long time, which means there are tons of tools, resources, and tutorials (shoutout to Shubhra Ma’am’s PPTs) to help you out.

### Cons:
- **Scaling is a Headache:** Vertical scaling (adding more resources to a single server) is the norm here, which can be expensive and difficult as your app grows. Horizontal scaling (like MongoDB’s chill vibe) is trickier.
- **Rigid Structure:** If you don’t plan your database schema properly, you’re in for a world of hurt when changes come down the line. You can’t just toss in a new field like you can with MongoDB.

### Best For:
- **Large-scale apps** with complex data relationships and a need for reliability and structure. Perfect for projects where data needs to be consistent and relational.

---

## Firebase 🔥

![Firebase Logo](assets/firebase.jpg)

Firebase is like the cool, modern, serverless database that’s all about convenience. It’s hosted in the cloud by Google (yeah, that Google). You don’t have to worry about managing servers or anything like that—just focus on your app and let Firebase handle the rest.

### Pros:
- **Serverless OP:** No need to spin up servers or maintain anything—Firebase does all that for you. Just connect, and boom, you’ve got a database.
- **Real-time Updates:** Firebase syncs data in real-time, making it perfect for chat apps, live notifications, or anything where data needs to be instantly up-to-date.
- **Authentication Built-In:** It comes with built-in user authentication services, so no need to go find a separate solution for that. Shoutout to Firebase Auth for saving us from yet another headache!

### Cons:
- **Scaling Struggles:** It’s all fun and games until your app blows up in popularity (in a good way, hopefully) and you start hitting Firebase’s scaling limits. You might find it tricky to manage performance when you have a ton of users.
- **Pricing Feels Like a Plot Twist:** It’s free for small projects, but as you scale up, the pricing can hit you like that surprise quiz from Shubhra Ma’am. Startups might feel the pinch when those bills roll in.

### Best For:
- **Startups or small projects** where you want to get up and running fast without worrying about server stuff. If your app’s going to be a simple chat app or a student project, Firebase has your back.
