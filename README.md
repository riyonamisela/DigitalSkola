# DigitalSkola#Flask Dengan Sqlalchemy

##Install SQL Alchemy for Flask
pip install -U Flask-SQLAlchemy

##Masuk CLI ketik python


##ketik perintah di bawah ini

from BasicApi import db
db.create_all()

from BasicApi import User
raymonde = User (name ='Raymonde N. Lopez', email ='RaymondeNLopez@teleworm.us', dob ='1988-03-18', age=33 )
thais= User (name ='Thais Ferreira Azevedo', email ='ThaisFerreiraAzevedo@teleworm.us', dob ='1958-11-02', age= 63)
kornelis= User (name ='Kornelis van Egmond', email ='KornelisvanEgmond@dayrep.com', dob ='1978-03-18', age= 43)

db.session.add(raymonde)
db.session.add(thais)
db.session.add(kornelis)
db.session.commit()

##Untuk mengakses data
User.query.all()
