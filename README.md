# Alibaba-Marketplace : An ECommerce Website like Alibaba.com


  1. create Heroku Account
  2. create new App
  3. git remote add heroku https://git.heroku.com/myamazona.git
  4. Install Heroku CLI
  5. heroku login
  6. git push heroku master
  7.  create https://www.mongodb.com/cloud 
  8.  create database and copy connection string
  9.  add MONGODB_URL to config var of heroku
  10. add PAYPAL_CLIENT_ID to config var of heroku
  11. Update package.json  
  12. "build": "rm -rf dist && babel backend -d dist",
  13. "heroku-postbuild": "npm run build && cd frontend && npm install && npm run build"
  14. "engines": { "node": "12.4.0", "npm": "6.9.0"}
  15. Procfile web: node dist/server.js
