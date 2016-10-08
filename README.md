LOUNCH

1). Insert in you rails application this file and change you Gemfile and Gemfile.lock (should be you).

2). In Dockerfile and docker-compose.yml set name you application ("shop" change to name you application)- will be for example:
  volumes:
    - .:/site
  
    ADD . /site

3). Lounch
     - docker-compose up


HOW USE
  
1). Migrate database or create scaffold:
      - docker-compose run web rake db:migrate
      - docker-compose run web rails g scaffold Article title content 

2). Update Gemfile
      - docker compose build


EDIT APPLICATION (example see in console " A server is already running. C" should delete tmp/pids/server.pid) for lounch application
  
  1). Use this command ()
      sudo chown -R $USER:$USER .
     
     and then delete tmp/pids/server.pid

 
Questions?

Have a look at our FAQs for users, for pod administrators or for developers.

Still haven't found an answer? Talk to us! Read how we communicate. We're here to answer all your questions.

Contribute

To keep game* growing and improving we need all help we can get. Whether you can contribute code, ideas,translations,bug reports or simply extend the community as a helpful user or pod administrator, your help is welcome!

Everyone interacting in game codebases, issue trackers, chat rooms, mailing lists, the wiki,game and the Loomio group is expected to follow the game* code of conduct.

Security

Found a security issue? Please disclose it responsibly. We have a team of developers listening to support@everprin.com. The PGP fingerprint is AB0D AB02 0FC5 D398 03AB 3CE1 6F70 243F 27AD 886A.
