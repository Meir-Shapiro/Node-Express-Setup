cd /vagrant
sudo npm install express-generator -g
sudo express project
cd project
sudo npm install

DEBUG=project:* npm start

Vagrant
	vb.customize ["setextradata", :id, "VBoxInternal2/SharedFoldersEnableSymlinksCreate/v-root", "1"]
	http://blog.rudylee.com/2014/10/27/symbolic-links-with-vagrant-windows/
	
http://tasks.ltccs.dev:3000/