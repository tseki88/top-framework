# CSS-Grid-Framework

### Based off: The Odin Project - Design Your Own Grid-Based Framework

This is my implementation of a 16-grid CSS framework.
Main purpose of this project is to demonstrate my understanding on the basics of how frameworks such as Bootstrap was built.

#### Guidelines to Follow:

Begin by importing `framework.css` from this repository into your HTML file.

This framework is utilized by specifying the number of columns to cover (totalling to 16) within each row of `class="row"` that is nested in the parent container div of `class="container"`.

```html
<body>
    <div class="container">
        <div class="row">
        </div>
        <div class="row">
        </div>
    </div>
</body>
```

The amount of columns each div within the row (out of max 16) takes up can be specified by providing a `class="col-width-X"`, where **"X"** is a number between 1 and 16.


#### Reminder:
If the total col-width within the row is below 16, there will be blank spaces left with nothing to occupy rest of the width.
If the total col-width within the row exceeds 16, each col-width prior to that will be squished to accommodate for the extra columns and will no longer adhere to the grid layout.


#### Example in Use:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="framework.css">
</head>
<body>
    <div class="container">
        <div class="row">
            <div class="col-width-2 pink">Hi</div>
            <div class="col-width-4 blue">This is a Title</div>
            <div class="col-width-4 pink"></div>
            <div class="col-width-2 green">Maybe</div>
        </div>
        <div class="row">
            <div class="col-width-1 purple">1</div>
            <div class="col-width-2 pink">2</div>
            <div class="col-width-5 red">5</div>
            <div class="col-width-8 blue"></div>
        </div>
    </div>
</body>
</html>
```
![Example Screen](./demo-screenshot.png)