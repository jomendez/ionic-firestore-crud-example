# ionic-firestore-crud-example
Simple CRUD (Create, Read, Update and Delete) using ionic 3 and Cloud firestore

![image](https://user-images.githubusercontent.com/8228498/79777514-5c030b80-8305-11ea-9419-49a67dd317c5.png)

In this project we are going to create the most simplest ionic CRUD (Create, Read, Update and Delete) using Cloud firestore. 

### You can find the full tutorial [here](http://www.jomendez.com/2018/03/09/ionic-crud-application-cloud-firestore/) 

At the end of this tutorial you\'ll be able to: 

- Setup a firebase account. 
- Configure firestore database permissions. 
- Create an ionic app using ionic cli (command line tool). 
- Create, Read, Update and Delete to a firestore database from an ionic app. 

## Run the ionic CRUD project.

First, install [Node.js](http://nodejs.org/). Then, install the latest Cordova and Ionic command-line tools in your terminal. Follow the [Android ](https://cordova.apache.org/docs/en/latest/guide/platforms/android) and [iOS ](https://cordova.apache.org/docs/en/latest/guide/platforms/ios) platform guides to install required tools for development. For more info go here: [https://ionicframework.com/getting-started](https://ionicframework.com/getting-started). 

```
npm install -g cordova ionic
```

Now lets create the ionic app 

```bash
git clone https://github.com/jomendez/ionic-firestore-crud-example.git
cd ionic-firestore-crud-example
ionic serve
```

## What is cloud firestore?

[![firestore youtube](http://img.youtube.com/vi/QcsAb2RR52c/0.jpg)](http://www.youtube.com/watch?v=QcsAb2RR52c "")

## Lets set up a firebase account.

Go to [https://console.firebase.google.com](https://console.firebase.google.com) and login with your google account or create one. 

![firebase new project](https://user-images.githubusercontent.com/8228498/79777692-9bc9f300-8305-11ea-86e4-a7f9569d37c9.png)

Enter the name of the project and click on Add Firebase to your web app.

![firebase configuration](https://user-images.githubusercontent.com/8228498/79777791-c6b44700-8305-11ea-8816-746c87bd5081.png)

We are going to use this data later, this will allow us to connect to firebase. 

Next step is to configure Cloud Firestore, follow the following steps in the image, and start in test mode for now, to keep it simple. 

![configure firestore database](https://user-images.githubusercontent.com/8228498/79781318-4db7ee00-830b-11ea-8f49-8b8f05d37d89.png)

For more rules you can visit here: [https://cloud.google.com/firestore/docs/security/rules-query](https://cloud.google.com/firestore/docs/security/rules-query)


Before we get into the ionic part, lets see how a firestore database structure looks like: 


![cloud firestore content](http://www.jomendez.com/wp-content/uploads/2018/03/cloud-firestore.gif)

This example was taken from the [ionAppFull4Pro](https://www.jomendez.com/ionic-boilerplate-full-app/) ionic starter. 
In this example you can see that the firestore data model is based on collections and documents, and you can nest collection within documents: 

![firestore structure](https://user-images.githubusercontent.com/8228498/79781673-d20a7100-830b-11ea-8ade-b3af2b2f96e8.png)

for more details you can visit here [https://firebase.google.com/docs/firestore/data-model](https://firebase.google.com/docs/firestore/data-model). 

