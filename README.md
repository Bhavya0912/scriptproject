# Mathematical Calculations using JavaScript
## AIM:
To design a website to calculate the area of a circle and volume of a cylinder using JavaScript.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Write JavaScript to perform calculations.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.


## PROGRAM:
### mathvolume.html
```
{% load static %}
<!DOCTYPE html>
<html lang=en>

<head>
    <title>VOLUME OF THE CYLINDER</title>
    <link rel="stylesheet" href="{% static 'css/mathscript.css' %}">
</head>

<body>
    <div class="container">
        <div class="formview">
            <div class="banner">
                VOLUME OF A CYLINDER
            </div>
            <div class="content">
                <form action="/mathvolume/" method="POST">
                    {% csrf_token %}
                    <div class="forminput">
                        <label for="value_radius">RADIUS=</label>
                        <input type="text" name="value_radius" id="value_radius" value="{{radius}}">
                    </div>
                    <div class="forminput">
                        <label for="value_height">HEIGHT=</label>
                        <input type="text" name="value_height" id="value_height" value="{{height}}">
                    </div>
                    <div class="forminput">
                        <button type="submit" name="button_volume" id="button_volume">calculate volume</button>
                    </div>
                    <div class="forminput">
                        {{result}}
                   </div>
                </form>
            </div>
        </div>
    </div>
    <script src="/static/js/mathscript.js"></script>
</body>

</html>

```

### matharea.html
```
{% load static %}
<!DOCTYPE html>
<html lang=en>

<head>
    <title>AREA OF CIRCLE</title>
    <link rel="stylesheet" href="{% static 'css/mathscript1.css' %}">
</head>

<body>
    <div class="container">
        <div class="formview">
            <div class="banner">
                AREA OF CIRCLE
            </div>
            <div class="content">
                <form action="/matharea/" method="POST">
                    {% csrf_token %}
                    <div class="forminput">
                        <label for="value_radius">RADIUS=</label>
                        <input type="text" name="value_radius" id="value_radius" value="{{radius}}">
                    </div>
                    <div class="forminput">
                        <button type="submit" name="button_area" id="button_area">calculate area</button>
                    </div>
                    <div class="forminput">
                        {{result}}
                   </div>
                </form>
            </div>
        </div>
    </div>
    <script src="/static/js/mathscript1.js"></script>
</body>

</html>
```

## OUTPUT:
![output](./static/img/OUTPUT1.jpg)
![output](./static/img/OUTPUT2.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/REPORT1.jpg)
![output](./static/img/REPORT2.jpg)


## RESULT:
Thus a website is designed for the Mathematical Calculations using JavaScript and is hosted in the URL http://bhavya.student.saveetha.in:8000/mathvolume. HTML code is validated.

Thus a website is designed for the Mathematical Calculations using JavaScript and is hosted in the URL http://bhavya.student.saveetha.in:8000/matharea. HTML code is validated.
