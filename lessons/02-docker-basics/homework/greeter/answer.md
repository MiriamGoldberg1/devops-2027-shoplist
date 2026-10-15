1:  docker build -t greeter:v1
2:  docker run -d --p 9000:8000 --name greeter greeter:v1
3:  docker run -d -p 9000:8000 -e GREETING=Shalom 
4:  "Shalom, Rivka!"
5: השורות שיסומנו כCACHED ולא ררוצו שוב: כל השורות שכתובות לפני השורה ש בההשינוי
5: השורות שירוצו שוב: כל השורות שכתובות אחרי השורה שבה השינוי

