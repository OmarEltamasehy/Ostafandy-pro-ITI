
# **Ostafandy Web Application**

### *Description:*
Ostafandy is a [Django](https://www.djangoproject.com/)-Based Web Application providing a Marketplace for Handymen to support Home Services.

### *System Architecture*

<p align="center">
  <a href="https://nodejs.org/">
    <img alt="Node.js" src="/home/hakeem/Desktop/SystemArch.png" width="550" height="200"/>
  </a>
</p>


### *Usage:*
you can use this application in two different ways.

* As a Client

once you registerd as a client then you can order a craftsman by determining type of the problem you face then we will suggest some nearby craftsmen and what should you do is just select a one of them 

* As a Craftsman "Ostafandy"

once you registerd as a Craftsman or Ostafandy, what you should do is to till us every day if you are avaliable today of not to help us make you appear in craftsmen search result to the clients



### *Installtion*

* Clone this repo to your local machine using `https://github.com/OmarEltamasehy/Ostafandy-pro-ITI`

* Setup Docker Engine and Docker Compose from [here](https://docs.docker.com/install/).

### *Docker Commands to run the project*

```console
$ docker-compose -f docker-compose.prod.yml up -d --build
```
```console
$ docker-compose -f docker-compose.prod.yml exec web python manage.py createsuperuser
```
```console
$ docker-compose -f docker-compose.prod.yml exec web python manage.py makemigrations
```
```console
$ docker-compose -f docker-compose.prod.yml exec web python manage.py migrate --noinput
```
```console
$ docker-compose -f docker-compose.prod.yml exec web python manage.py collectstatic --no-input --clear
```
```console
$ docker-compose down -v
```

### *directory & file structures*

├── .env.dev

├── .env.prod

├── .gitignore

├── Ostafandy

│   ├── Dockerfile

│   ├── Dockerfile.prod

│   ├── entrypoint.prod.sh

│   ├── entrypoint.sh

│   ├── Ostafandy

│   │   ├── _init_.py

│   │   ├── settings.py

│   │   ├── urls.py

│   │   └── wsgi.py
     
|   ├── custmores

│   │   ├── _init_.py

│   │   ├── settings.py

│   │   ├── urls.py

│   │   └── wsgi.py

│   ├── manage.py

│   └── requirements.txt

├── docker-compose.prod.yml

├── docker-compose.yml

└── nginx
    ├── Dockerfile
    └── nginx.conf
  



### *Contributing & Advanced Developers*
For anyone wishing to contribute to Ostafandy or to customise core files feel free to submit pull requests to help in:

* Fix errors
* Improve sections
* Add new sections
* Content that needs some polishing is placed under development.

*just do the following:*

1. Fork it ( "https://github.com/OmarEltamasehy/Ostafandy-pro-ITI" )
2. Create your feature branch (git checkout -b my-new-feature)
3. Commit your changes (git commit -am 'Add some feature')
4. Push to the branch (git push origin my-new-feature)
5. Create a new Pull Request


### *Roadmap*

In the next release we will add more features like:

1. application will support english.
2. application will available throughout the Arab world.
3. add rating feature.



### *Security Vulnerabilities*
If you discover a security vulnerability within Ostafandy, please send an e-mail to ostafandysupport@gmail.com. All security vulnerabilities are reviewed on a case-by-case basis.

### *Copyright & License*
Copyright (c) 2019 Ostafandy Foundation - Released under the <a href="http://www.iti.gov.eg/Site/Home" target="_blank">ITI</a> license. Ostafandy and the Ostafandy Logo are trademarks of Ostafandy Foundation Ltd. Please see our trademark policy for info on acceptable usage.
