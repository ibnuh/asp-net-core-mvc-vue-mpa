#  ASP.NET Core MVC + Vue Multi Page Application

![enter image description here](https://lh3.googleusercontent.com/gjq_nmo7smL0CtbaD-3KRPA7Vq55Phz9kVR9CkybFytt49bOXBpsiIh4Do3iLrjOt8ejxob_5j7u "ASP.NET Core MVC + Vue Multi Page Application")

Highly scalable, quick scaffolding, customizable and easy to setup starting point for ASP.NET Core MVC using Razor Page and Vue.

##  Installation
```
# 1. Clone the repository
git clone https://github.com/ibnuh/asp-net-core-mvc-vue-mpa.git my-new-project

# 2. Go to the cloned repo folder
cd my-new-project

# 3. Install dependencies
npm install
```

##  Architecture
This architecture is 100% inspired by [Laravel's JavaScript & CSS Scaffolding](https://laravel.com/docs/5.8/frontend).

|Path|Description|
|--|--|
|`/Vue`|Where all the frontend related code lives, you can customize it as you wish.|
|`/Vue/app.js`|Entry point for our Vue.js application. You should customize this file for your needs.|
|`/Vue/components`|Where most of the components in our app will live, subfolder allowed.|
|`/webpack.mix.js`|Config file for [Laravel Mix](https://github.com/JeffreyWay/laravel-mix), it's *a clean layer on top of webpack to make the 80% use case laughably simple to execute.* You can see the [documentation](https://laravel-mix.com/docs) for more information.
|`wwwroot/dist`|Output for our compiled resources, you can customize this by editing the laravel mix config file.|

## How to use
Laravel Mix provides a clean npm to speed up our workflow.

### Start a watcher
The files inside `/Vue` folder will be automatically compiled when the watcher detect changes.
```
npm run watch
```

### Compile codes for development use
```
npm run dev
```

### Compile for production use
This command will minify and optimize our codes for production use
```
npm run prod
```

##  Sample Usage

You can have a look at these files below

 - `/Views/Home/Index.cshtml`
 - `/Vue/components/CookieConsent.vue`
