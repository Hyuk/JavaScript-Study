# Basics
* in-line comment
* multi-line comment 
* inline javascript in html
* external javascript file in html

### in-line comment
```javascript
// this is an in-line comment
```

### multi-line comment
```javascript
/* this is a
multi-line comment */
```

### how to use javascript in HTML file - inline
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <script type="text/javascript">
    console.log('JavaScript');
  </script>
</body>
</html>
```

### how to use javascript in HTML file - external file
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title>
</head>
<body>
  <script src="http://code.jquery.com/jquery.js"></script>
</body>
</html>
```

### Semi Colon at the end of javascript code
* The semicolon can be omitted but it has to be at the end of the javascript code
```javascript
console.log('JavaScript');
```

### Code can be written in multipleline
```javascript
console
.
log
(
  'Hello World'
);

// Hello World
```

### Code can't be written in multipleline
break, continue, throw, ++, --


### Code can be one line
```javascript
console.log('smart'); consol.log('Hello World');
```