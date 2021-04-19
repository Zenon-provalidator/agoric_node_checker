# Install
npm install

npm install -g pm2

cp exam_config config

# Control
pm2 start ./app.json

pm2 stop agoric_node_checker

pm2 delete agoric_node_checker

# Log
tail -f ./log/agoric_node_checker.log

tail -f ~/.pm2/logs/agoric_node_checker-error.log
