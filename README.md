# steward-websites

## Usage
> Steward Version >= v3.5.3

### install
`wsm install`

### uninstall
`wsm uninstall`

## Contributing
Add the configuration of the website to the data.json file

### website data structure
> Please remove the comments

```javascript
{
    "author": "solobat", // required
    "version": 1, // required
    "host": "sspai.com", // required
    "icon": "https://cdn.sspai.com/sspai/assets/img/favicon/icon.ico",
    // Specify the area to extract the outline
    "outlineScope": ".article-content", // [jquery] css selector
    // Generate navigations
    "navs": "nav a", // [jquery] css selecotr
    // Supplement to `navs`
    "paths": [
        {
            "title": "首页",
            "urlPattern": "/" // path
        },
        {
            "title": "个人主页",
            "urlPattern": "/user/784469/posts"
        }
    ],
    "title": "少数派"
},
```