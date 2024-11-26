# Data_based_ Workshop
In this workshop, students will explore the fundamental concepts behind databases, and then practice creating and updating a database of their own. They will briefly learn about relational databases, SQL, NoSQL, and the importance and impact of databases in modern society. By the end of the workshop, each student will have access to their own database, and will be able to interact with it in multiple ways.

## Workshop Outline
The workshop consists of these parts:

### Presentation
Present the [PowerPoint](DataBasedPresentation.pptx). These slides contain a brief introduction to data and databases, including SQL and NoSQL design approaches. There are notes with talking points in the slides.

### Follow-Along
Walk through the [Follow-Along Activity](FollowAlong.md) with the students. They should create and deploy their own cluster in MongoDB Atlas, and then connect to it through a web application.

#### Starter Project: Web Application
[Click here to remix the web application project on Glitch.](https://glitch.com/edit/#!/remix/hh25-posts-db)

#### Back-up Connection String
If a student is _really_ struggling to follow along with the activity, this connection string can be shared with them. Replace `<username>` with `ezekieljohnson`, and `<password>` with `eM4OPS9FdgsAVLpV` in this string:

```
mongodb+srv://<username>:<password>@cluster0.6haikte.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
```

If a student does use this connection string, they can still create their own personal database within the cluster. In the **server.js** file, on line **25**, they can change the `dbsettings.dbName` property to point to something new - like `"posts-alice"` or `"posts-bob"`. It should look something like this:

```js
dbSettings.dbName = "posts-student-name-here";
```

### Gimkit
[Gimkit](https://gimkit.com/) is a fun formative assessment tool that's similar to Blooket, but with some different game modes. Just like Blooket, there are a variety of modes where the students compete against each other in different ways. Answering questions correctly helps them achieve more success in each game.

An account is required to host the game; here are some credentials you can use:

- Username: **techoutreachinstructor@gmail.com**
- Password: **Tech0utreach!**

When setting up the game, try to time it so that it ends just a couple minutes before the camp ends. Note that it will likely take 2-3 minutes for all the students to join the game, so a game time limit of **7 minutes** might end up taking about **10 minutes**.

1. Go to the [Gimkit Login Page](https://gimkit.com/login)
1. Enter the credentials above
1. Find the [**Databases** question set](https://www.gimkit.com/view/66464769fa43d1810473acde)
    - If it appears in the list, click the green "Play Live" button
    - From the set page, click the "Play Live" link on the left side
1. Select one of the freely-available game modes
1. Adjust the time as needed, but keep everything else the default
1. Click the **Continue** button
1. Instruct students to go to **gimkit.com/join**, enter the code and a nickname, and join the game
1. Once all students have joined, click the **Start Game** button

From there, the students will work on their own, answering questions and trying to win the game!

## Agenda

| Activity | Time |
|-|-|
| Presentation | 10m |
| Follow-Along | 40m |
| Gimkit | 10m |
