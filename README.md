# Grid-Based Framework

### Based off: The Odin Project - Design Your Own Grid-Based Framework

This is my implementation of a 16-grid CSS framework.
Main purpose of this project is to demonstrate my understanding on the basics of how frameworks such as Bootstrap was built.

#### Guidelines to Follow:

Begin by importing `framework.css` from this repository into your HTML file.

**Notes:**
 - Gap is set to a default of 10px.
 - Min-height of each row is set to 25px.

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
Please checkout index.html within repository of this framework used to recreate Juno's home page [www.junocollege.com]. (in progress)