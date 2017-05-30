## Generating an Express App for Elastic Beanstalk

    npm install -g express-generator
    express --view=pug express-beanstalk
    mv ./bin/www ./www.js
    edit www.js to update relative path for app.js

## Running Express App on Elastic Beanstalk

    brew install awsebcli
    eb init -r us-east-1 -p "Node.js"
    eb create
    eb deploy
