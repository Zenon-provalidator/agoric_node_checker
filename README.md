##install
npm install

npm install -g pm2

cp exam_config config

pm2 start ./app.json

pm2 stop agoric_node_checker

pm2 delete agoric_node_checker



##show log
tail -f ./log/agoric_node_checker.log

##show pm2 error log
tail -f ~/.pm2/logs/agoric_node_checker-error.log
