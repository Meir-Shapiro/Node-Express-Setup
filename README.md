1. vagrant up
2. cd /vagrant
3. sudo npm install express-generator -g
4. sudo express project
5. cd project
6. sudo npm install

DEBUG=project:* npm start //to run server and listen

### Make sure to add to Vagrant file
	vb.customize ["setextradata", :id, "VBoxInternal2/SharedFoldersEnableSymlinksCreate/v-root", "1"]
http://blog.rudylee.com/2014/10/27/symbolic-links-with-vagrant-windows/
	
### Set up Hosting file and go to following url
http://tasks.ltccs.dev:3000/
