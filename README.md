# 30DAYSOFGOOGLE-CLOUD-LEADERBOARD
Shows top 20 participant list according to the number of badges earned.

To Run this Application in your file you must have install redis
1. start redis server  
2. make a virtual env with python >= 3.7  
3. install requirements.txt
4. run `python manage.py migrate`
5. run `python manage.py runserver`
6. run in another terminal `celery -A challenge_leaderboard worker -l INFO --beat` for linux users and for windows users run  
```
celery -A challenge_leaderboard worker -l info -P gevent  
celery -A challenge_leaderboard beat -l info  
```

### You can change the beat time in the `challenge_leaderboard/celery.py` file

# Sample
https://github.com/GDGVIT/cloud-program-leaderboard-frontend/pull/1

https://github.com/GDGVIT/cloud-program-leaderboard

Check it out - 
 https://30daysofgcp-asiet.netlify.app/



Also GitHub link if you wanna use this project 
 https://github.com/theharshitkumar/30daysleaderboard
