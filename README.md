## Getting started

This is a simple starter template for building and running an app using [Svelte](https://v3.svelte.technology). To get going, make sure you have [NodeJS](https://nodejs.org/en/) and [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) installed on your machine.

Next, `cd` to the directory where this project has been cloned...

```
git clone https://github.com/ganochenkodg/svelte-template.git
cd ./svelte-template
```

...install all project dependencies...

```
npm install
```

...and run it for developing...

```
npm run dev
```

...or build the application.

```
npm run build
```

Also it have Dockerfile for dockerize your app.


```
docker build -t svelte-template ./
docker run -p 80:8080 svelte-template
```

![](https://github.com/ganochenkodg/svelte-template/blob/master/svelte.png)
