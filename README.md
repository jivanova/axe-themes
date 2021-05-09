### Kendo-Themes Repo setup

1. Repo setup

```
npm install
npm run bootstrap
npm run sass
npm run visual-tests // will start tests through http-server `http://127.0.0.1:8080/tests/visual/`
```

2. Pages setup

Remove the background for pages to be sure that clean pages with the components are tested.

> kendo-themes > tests > visual > assets > styles.css

``` css
/* Shades of gray*/
.k-bg-gray-50  { }
.k-bg-gray-100 { }
.k-bg-gray-200 { }
.k-bg-gray-300 { }
.k-bg-gray-400 { }
.k-bg-gray-500 { }
.k-bg-gray-600 { }
.k-bg-gray-700 { }
.k-bg-gray-800 { }
.k-bg-gray-900 { }
```

### Axe testing

1. Download chromedriver from:

https://chromedriver.storage.googleapis.com/index.html
https://chromedriver.storage.googleapis.com/index.html?path=90.0.4430.24/ - might use this one if the version is a match

2. Update Path environment variable to point to the location of the chromedriver.exe

3. Repo setup

``` 
npm install
node index
```

The above command will generate the results files in results > material folder.