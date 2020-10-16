## BUCKKET-LIST-MEVN 
## Project Peek:
Demo link: [mevn-bucket-list-app1](https://mevn-bucket-list-app1.herokuapp.com/)

To run the project in the local:

npm install 

1,connct the database:  
```
export MONGO_URI='mongodb+srv://88888888:XXXXXX@cluster0.vbecz.mongodb.net/test?retryWrites=true&w=majority'

echo $MONGO_URI
```
2.npm run dev the project:
```
npm run dev
```

## Prject Bug  handling:

1.[Homebrew国内如何自动安装（国内地址](https://zhuanlan.zhihu.com/p/111014448)  

### MongDB Database:
2.Mongoo Account : Google account 

[MongoAtlas](https://cloud.mongodb.com/v2/5f8737ed76b45308cd24df78#security/database/roles)  
3.You need to stop the Mongodb, if you are using the community version of the mongodb, you couold stop it in the terminal or visula studio terminal  
[Install MongoDB Community Edition on macOS](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/)  
4.make sure that between "npm run server" and \" leave a space to avoid the error happend  

5.Connect to your application: 
1.The process to run your Mongodb:  
```
export MONGO_URI='mongodb+srv://88888888:XXXXXX@cluster0.vbecz.mongodb.net/test?retryWrites=true&w=majority'

echo $MONGO_URI

node server.js
```

2. Explain the content
```
mongodb+srv://88888888:<password>@cluster0.vbecz.mongodb.net/<dbname>?retryWrites=true&w=majority
```
mongodb+srv://username:<password>@clusterurl<dbname>?retryWrites=true&w=majority
username: 88888888aDatabase Access;
password: You could see it from the Database Access
url: connect the clauster and connection method and choose the connect to your application, you will find out.
<dbname>:You need to give a one

6.Node / Express: EADDRINUSE, Address already in use - Kill server
```
lsof -i tcp:3000
kill -9 5805
```
[Node / Express: EADDRINUSE, Address already in use - Kill server](https://stackoverflow.com/questions/4075287/node-express-eaddrinuse-address-already-in-use-kill-server)

7.If you meet can not resolve the host name, Make sure you add the: after the http:
```
http://localhost:3000/api/bucketListItems
```
[Insomnia Core download](https://insomnia.rest/download/#mac)
8. To add the emojy into the text, you could copy the emoj to the text to do it:
[eomoj search](https://getemoji.com/#food-drink)  

To delet the a item, you need to copy the id into the url and do not add the " to the url, the content in the JSON part needs to 
be deleted too:
```
http://localhost:3000/api/bucketListItems/5f881bbb743402f1e6ddc34b
```
### 9. To run the project, you need to connct the database first,. then npm run dev the project. The process will be like below:
1,connct the database:  
```
export MONGO_URI='mongodb+srv://88888888:XXXXXX@cluster0.vbecz.mongodb.net/test?retryWrites=true&w=majority'

echo $MONGO_URI
```
2.npm run dev the project:
```
npm run dev
```
3.You need to clean the hello world import and component in the App.vue;  

10. if you could not see the content list in the browser, you need to check if you wtite the "mounted" correctly in the App.vue file:
```
async mounted() {

    const response = await axios.get('api/bucketListItems/')
    this.items = response.data;
  }
```

if you could not click the 'addItem' in the browser, You need to check it in the click and method in the App.vue file, make usre that they are the same.

### Heroku Deploy project:  
11. if you see your code could not run out the content and told you iselected is not defined, make sure that to go to the App.vue file to check the Curly braces, make sure that there is no extra or lack of curly brace.  

12. install the Heroku cli, you need to select the mobile data to process it.  

13. Login heroku it with the mobile data, if your heroku login doese not work.   

Heroku official link: [Heroku](https://dashboard.heroku.com/)

### Lerning resource:
1.Video: [Full Stack Vue App: Learn MEVN in one video with Mongo Express Vue and Node js](https://www.youtube.com/watch?v=vr6O-IYebXA&list=PLul9aZOSt5CPetBw-Nl_6PzdgG-bBYL75&index=3&t=137s&ab_channel=EstebanCodes)  
2.Source Code:[bucket-list-mevn](https://github.com/3stbn/bucket-list-mevn/pulls)  