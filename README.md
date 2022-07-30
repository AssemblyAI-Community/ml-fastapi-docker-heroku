
Create Docker container:

```
docker build -t app-name .

docker run -p 80:80 app-name
```

Create Git repo (if you clone this repo this step is not needed):

```
git init
git add .
git commit -m "initial commit"
```

Create Heroku project

```
heroku login
heroku create your-app-name
heroku git:remote your-app-name
heroku stack:set container
git push heroku main
```