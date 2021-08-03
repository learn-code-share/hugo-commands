# hugo-commands

For more information, visit [official documentation](https://gohugo.io/getting-started/quick-start/)

Prerequisites 
- NodeJS
- Git
- Hugo

Create new site
```
hugo new site quickstart
```

add a theme
```
cd quickstart
git init
git submodule add <theme git url>
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke

// Update the config.toml file to use the theme
theme = "ananke"
```
Update config.toml file will look something like
```
baseURL = "https://jitangupta.com/"
languageCode = "en-us"
title = "Full Stack Engineer | Jitan Gupta"
theme = "ananke"
```
Add Content
```
hugo new posts/first-post.md
```
Above command will create a file as show below
![image](https://user-images.githubusercontent.com/11292363/127779296-16b84204-8fa5-42c2-a775-389434ca07d9.png)

Start hugo server
```
hugo server -D
```

Build static pages
```
hugo -D
```
Output will be in `./public/` directory by default (`-d`/`--destination` flag to change it, or set `publishdir` in the config file).

---
# Hugo Custom Theme
Creating a new theme hugo is verify simple as below

```
1//
hugo new site custom-theme
cd custome-theme

//2
hugo new theme todu-theme
```
Your theme is now created
You can update config.toml
![image](https://user-images.githubusercontent.com/11292363/127973788-f6a4792f-12d9-42fe-954c-54877d875753.png)

