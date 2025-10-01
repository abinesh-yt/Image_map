# Ex04 Places Around Me
# Date: 01-10-2025
# AIM
To develop a website to display details about the places around my house.

# DESIGN STEPS
## STEP 1
Create a Django admin interface.

## STEP 2
Download your city map from Google.

## STEP 3
Using <map> tag name the map.

## STEP 4
Create clickable regions in the image using <area> tag.

## STEP 5
Write HTML programs for all the regions identified.

## STEP 6
Execute the programs and publish them.

# CODE

map.html
```
<!DOCTYPE html>
<html>
<head>
    <title>Places Around My House</title>
</head>
<style>
    p{
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    }
    h1{
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
    }
    
  
</style>
<body style="background: linear-gradient(to left ,  skyblue, white); " >
    <center>
    {% load static %}
    
    <h1 style="color: black;">Places Around My House</h1>
    <p>Click on the marked areas in the map to see details about each place.</p>

    <img src="{% static 'map.png' %}" usemap="#image-map" alt="My Area Map">

    <map name="image-map">
    <area shape="rect" coords="799,236,497,482" href="\place1\" alt="mountain" title="mountain">

    <area   title="vels institute of technology" href="\place2\" coords="687,571,395,827" shape="rect">

    <area  title="saravana store" href="\place3\" coords="113,691,383,817" shape="rect">

     <area   title="Zamin pallavaram" href="\place4\" coords="783,493,638,597" shape="rect">

      <area target="" alt="" title="pallavaram Railway station" href="\place5\" coords="372,371,536,467" shape="rect">
    </map>

    </center>
   

 
</body>
</html>
```


place1.html
```
<!DOCTYPE html>
<html >
<head>
    
    <title>mountain</title>
</head>
<style>
    img{
        height: 350px;
        width: 450px;
    }
    h1{
        color: aqua;
        height: 70px;
    }
    p{
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>
<body style="background: linear-gradient(to left , green, lime  );">
    
    <a href="/">← Back to Home</a>
    <center>
    <h1>mountain</h1>
    {% load static %}
    <img src="{% static 'image.png' %}" alt="mountain">
    <p>Pallavaram Mountain is a historic hill located in Chennai, Tamil Nadu. It is known for its natural beauty, rocky landscape, and archaeological importance. The mountain offers scenic views of the surrounding city and is popular among hikers and nature lovers. Ancient stone tools and cave paintings have also been discovered here, proving its cultural heritage.</p>
    </center>
    
</body>
</html>
```

place2.html
```
<!DOCTYPE html>
<html >
<head>
    
    <title>vels</title>
</head>
<style>
    img{
        height: 350px;
        width: 450px;
    }
    h1{
        color: aqua;
        height: 70px;
    }
    p{
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>
<body style="background: linear-gradient(to left,#ff512f, #dd2476);">
    
    <a href="/">← Back to Home</a>
    <center>
    <h1>vels</h1>
    {% load static %}
    <img src="{% static 'vels.png' %}" alt="mountain">
    <p>Vels University, located in Pallavaram, Chennai, is a reputed institution offering a wide range of undergraduate, postgraduate, and research programs. The campus is known for its modern infrastructure, well-equipped laboratories, and experienced faculty. It emphasizes both academics and extracurricular activities, encouraging students to excel in studies, innovation, sports, and cultural events</p>
    
    </center>
    
</body>
</html>
```

place3.html
```
<!DOCTYPE html>
<html >
<head>
    
    <title>super store</title>
</head>
<style>
    img{
        height: 350px;
        width: 450px;
    }
    h1{
        color: aqua;
        height: 70px;
    }
    p{
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        color: cyan;
    }
    a{
        color: brown;
        background-color: yellow;
    }
</style>
<body style="background: linear-gradient(to left , navy, black );">
    
    <a href="/">← Back to Home</a>
    <center>
    <h1>super store</h1>
    {% load static %}
    <img src="{% static 'super store.png' %}" alt="mountain">
    
    <p>Saravana Stores
Saravana Stores in Pallavaram is a popular shopping destination offering a wide variety of products at affordable prices. From clothing and household items to jewelry and electronics, the store attracts customers from different parts of Chennai. Known for its budget-friendly options and wide collection, Saravana Stores is a trusted choice for families and daily shoppers.</p>
    </center>
    
</body>
</html>
```

place4.html
```

<!DOCTYPE html>
<html >
<head>
    
    <title>zamin pallavaram</title>
</head>
<style>
    img{
        height: 350px;
        width: 450px;
    }
    h1{
        color: aqua;
        height: 70px;
    }
    p{
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>
<body style="background: linear-gradient(to left , skyblue, lightgreen );">
    
    <a href="/">← Back to Home</a>
    <center>
    <h1>zamin pallavaram</h1>
    {% load static %}
    <img src="{% static 'zamin pallavaram.png' %}" alt="mountain">
    <p>Zamin Pallavaram is a well-known residential and commercial locality in Chennai, located near Pallavaram. The area is popular for its peaceful environment, schools, temples, and growing infrastructure. It is well connected by road and rail, making it convenient for daily commuters. With rapid urban development, Zamin Pallavaram is becoming a preferred location for families and businesses.</p>
    
    
    </center>
    
</body>
</html>
```

place5.html
```

<!DOCTYPE html>
<html >
<head>
    
    <title>pallavaram Railway station</title>
</head>
<style>
    img{
        height: 350px;
        width: 450px;
    }
    h1{
        color: aqua;
        height: 70px;
    }
    p{
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
</style>
<body style="background: linear-gradient(to left ,  red, pink );">
    
    <a href="/">← Back to Home</a>
    <center>
    <h1>pallavaram Railway station</h1>
    {% load static %}
    <img src="{% static 'pallavaram.png' %}" alt="mountain">
    <p>Pallavaram Railway Station
Pallavaram Railway Station is one of the busiest suburban stations in Chennai, located on the Chennai Beach–Chengalpattu line. It connects Pallavaram with major parts of the city and nearby towns. The station is widely used by daily commuters, students, and travelers. With its strategic location, it plays a vital role in Chennai’s suburban transport network.</p>
    
    
    </center>
    
</body>
</html>
```

views.py
```
from django.http import HttpResponse
from django.shortcuts import render

def index(request):
    return render(request, "map.html")

def place1(request):
    return render(request,'place1.html')

def place2(request):
    return render(request,'place2.html')
    

def place3(request):
    return render(request,'place3.html' )

def place4(request):
    return render(request,'place4.html')

def place5(request):
    return render(request,'place5.html')
```

urls.py
```
"""
URL configuration for myproject project.

The `urlpatterns` list routes URLs to views. For more information please see:
    https://docs.djangoproject.com/en/5.2/topics/http/urls/
Examples:
Function views
    1. Add an import:  from my_app import views
    2. Add a URL to urlpatterns:  path('', views.home, name='home')
Class-based views
    1. Add an import:  from other_app.views import Home
    2. Add a URL to urlpatterns:  path('', Home.as_view(), name='home')
Including another URLconf
    1. Import the include() function: from django.urls import include, path
    2. Add a URL to urlpatterns:  path('blog/', include('blog.urls'))
"""
from django.contrib import admin
from django.urls import path
from myapp import views

urlpatterns = [
    path("", views.index),                
    path('place1/', views.place1),         
    path('place2/', views.place2),
    path('place3/', views.place3),
    path('place4/', views.place4),
    path('place5/', views.place5),
    path('admin/', admin.site.urls),
]


```
# OUTPUT
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/55387036-212f-49ed-a454-8ed246ea9dfd" />
<img width="1946" height="1172" alt="image" src="https://github.com/user-attachments/assets/ef45c67f-a994-4338-8f7e-4d4ec8d07379" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/22ac0551-442f-4247-aa7c-a6326c562ca0" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/4ecdfbd5-e100-4c6a-8340-50f47bbbc564" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/6294e353-a30a-4b74-a995-354bad4498ee" />
<img width="1920" height="1119" alt="image" src="https://github.com/user-attachments/assets/ee6add18-44e5-48f2-a5aa-031a444cd7ec" />





# RESULT
The program for implementing image maps using HTML is executed successfully.
