# create a function and call it
```
 function loaded() {
 
 //window load
 }
 ```
 
# first add the window loaded code
```
window.addEventListener('load', function () {
//css
//js code goes here
}
```

# add js  code 
```
let jsImportArray = [
          "https://hspwidget.html5.run/index.js",
          "./assets/js/alljs.js",
        ];
        jsImportArray.forEach((item, index) => {
          console.log("js Import Started")
          let script = document.createElement('script');
          script.src = item;
          document.getElementsByTagName('head')[0].appendChild(script);
          console.log("js Import ended")
        })
        
 ```
 
 # for css
 ```
  let cssImportArray = [
          "@import url('https://hspwidget.html5.run/index.css');",
        ]

        cssImportArray.forEach((item, index) => {
          console.log("css import Started")
          let styles = item;
          let newSS = document.createElement('link');
          newSS.rel = 'stylesheet';
          newSS.href = 'data:text/css,' + escape(styles);
          document.getElementsByTagName("head")[0].appendChild(newSS);
          console.log("css import ended")
        })
```        

