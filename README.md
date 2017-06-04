## Usage

cd base/
ansible-playbook -i ../inventory --ask-vault-pass site.yml


#### 
random notes

playbooks we need
grav/
 * drop nginx config file in /etc/nginx/sites-avaliable or whatever
 * ^^ this should be a template that fills in a var with the server name
 * copy (curl?wget?) the grav (+admin) install into /var/www/vhosts/{{ servername e.g. "southsoundsda.org/" }}
 * check out the dsa grav theme into /var/www/vhosts/{{server name}}/themes??
 * run the grav command line tool to generate an admin user (or maybe even authors)
 * any grav file config that needs to happen
 * link nginx config file to /etc/nginx/sites-enabled
 * restart nginx
 * socialism happens
