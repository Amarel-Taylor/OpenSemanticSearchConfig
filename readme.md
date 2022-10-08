Use Amazon AMI debian-11-amd64-20220503-998

Launch on a server with at least 8GB of ram

sudo apt-get update

wget https://opensemanticsearch.org/download/open-semantic-search_22.03.04.deb

sudo dpkg --install open-semantic-search_22.03.04.deb

sudo apt-get -f install

Create security group with open ports for 22, 80, 443 (optional: 7474,  8983, etc)

Check if web server running by visiting http://<server.ip>/search/ (do not use https)

sudo apt-get install git

cd /var/lib/opensemanticsearch/

sudo git init

sudo git add --all

sudo git commit -a -m "Commit message"

sudo pip install django-upgrade

sudo git ls-files -- '*.py' | xargs sudo django-upgrade --target-version 4.0

sudo vi /var/lib/opensemanticsearch/thesaurus/models.py

Remove duplicate arguments “null=True”

sudo python3 manage.py makemigrations

sudo python3 manage.py migrate

sudo vi /var/lib/opensemanticsearch/visual_graph_explorer/templates/graph.html

Change to (% load static %)

Enable neo4j in etl and web interface

Install neo4j version 4.0 (DO NOT USE OTHER VERSIONS)

Go to neo4j to setup at 127.0.0.1:7474

Enable neo4j in etl

Update neo4j password in config
