# wekan.io
http://qiita.com/okamoai/items/a875b26abab7f18da7d1

mongod --dbpath C:\mongodb\data --logpath C:\mongodb\logs\mongodb.log

rem set MAIL_URL='smtp://user:pass@mailserver.example.com:25/'
rem set MAIL_FROM='wekan-admin@example.com'
set MONGO_URL=mongodb://127.0.0.1:27017/wekan
set ROOT_URL=https://127.0.0.1
set PORT=8080

cd wekan\bundle
node main.js



1. Run production code to confirm everything is working
2. Copy production code to a deploy folder to protect it during Demeteorizer activities
3. Run “demeteorizer” inside ..\deploy folder in Developer Command Prompt VS2012 to Demeteorize
4. Rename ..\deploy.demeteorizer folder “resources”
5. Run “npm install” inside bundle\programs\server (yellow = okay, red = bad)
* 6. Remove npm-bycrpt package from ..server\npm folder (delete manually)
* 7. run “npm install bcrypt” from ..programs\server
8. Copy bin folder containing DLLs for Node, Mongo
9. Run start script to confirm everything is working

1. Run production code to confirm it works
2. Open Developer Command Prompt VS2012 and run "demeteorizer" in deploy folder 
3. Rename.demeteorizer folder into “resources”
4. Run “npm install” inside bundle\programs\server (yellow = okay, red = bad)
5. Run "npm uninstall fibers && npm install fibers"
6. Run “npm uninstall bcrypt && npm install bcrypt”
7. Copy x86 bin folder containing from repo
