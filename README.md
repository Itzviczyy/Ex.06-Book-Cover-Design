# Ex.06 Book Cover Design
## Date: 22.11.2025

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Book Cover - Python Crash Course</title>
    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
        }
        body{
            min-height:100vh;
            display:flex;
            justify-content:center;
            align-items:center;
            background:radial-gradient(circle at top,#0f172a,#020617);
            font-family:system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
        }
        .cover{
            width:360px;
            height:540px;
            border-radius:18px;
            overflow:hidden;
            position:relative;
            box-shadow:0 25px 70px rgba(0,0,0,0.8);
            background:#020617;
            color:#e5e7eb;
        }
        /* top ribbon */
        .top-strip{
            position:absolute;
            top:18px;
            left:18px;
            padding:4px 12px;
            border-radius:999px;
            font-size:11px;
            letter-spacing:0.16em;
            text-transform:uppercase;
            background:rgba(15,23,42,0.8);
            border:1px solid rgba(148,163,184,0.7);
        }
        /* background art */
        .art{
            position:absolute;
            inset:0;
            height:62%;
            background-image:url("cover-bg.jpg"); /* keep this image in same folder */
            background-size:cover;
            background-position:center;
        }
        .gradient-overlay{
            position:absolute;
            inset:0;
            background:linear-gradient(to bottom,
                    rgba(15,23,42,0.1) 0%,
                    rgba(15,23,42,0.85) 65%,
                    #020617 100%);
        }
        .content{
            position:relative;
            height:100%;
            padding:32px 26px 26px;
            display:flex;
            flex-direction:column;
            justify-content:space-between;
        }
        .title-block{
            margin-top:70px;
            max-width:90%;
        }
        .subtitle-top{
            font-size:11px;
            letter-spacing:0.22em;
            text-transform:uppercase;
            color:#e5e7eb;
            opacity:0.85;
        }
        .main-title{
            margin-top:10px;
            font-size:30px;
            line-height:1.05;
            font-weight:800;
            letter-spacing:0.03em;
        }
        .main-title span{
            display:block;
            background:linear-gradient(120deg,#f97316,#facc15,#fb923c);
            -webkit-background-clip:text;
            color:transparent;
        }
        .tagline{
            margin-top:10px;
            font-size:13px;
            line-height:1.5;
            color:#cbd5f5;
        }
        .tagline span{
            color:#facc15;
            font-weight:600;
        }
        .bottom-area{
            position:relative;
        }
        .edition{
            font-size:12px;
            letter-spacing:0.18em;
            text-transform:uppercase;
            color:#f97316;
        }
        .divider{
            margin-top:6px;
            width:80px;
            height:2px;
            background:linear-gradient(to right,#f97316,#facc15);
            border-radius:999px;
        }
        .series{
            margin-top:12px;
            font-size:11px;
            text-transform:uppercase;
            letter-spacing:0.16em;
            color:#9ca3af;
        }
        .author-block{
            margin-top:20px;
            display:flex;
            align-items:center;
            justify-content:space-between;
        }
        .author-text{
            font-size:12px;
        }
        .author-label{
            text-transform:uppercase;
            letter-spacing:0.16em;
            font-size:10px;
            color:#9ca3af;
        }
        .author-name{
            margin-top:3px;
            font-size:15px;
            font-weight:700;
            letter-spacing:0.03em;
        }
        .author-photo{
            width:58px;
            height:58px;
            border-radius:999px;
            border:2px solid rgba(248,250,252,0.8);
            background:radial-gradient(circle at 30% 0%,#1f2937,#020617);
            display:flex;
            align-items:center;
            justify-content:center;
            font-size:22px;
        }
        .author-photo span{
            opacity:0.9;
        }
        .code-badge{
            position:absolute;
            right:0;
            bottom:0;
            font-size:9px;
            text-transform:uppercase;
            letter-spacing:0.18em;
            padding:4px 10px;
            border-radius:999px 0 0 0;
            background:linear-gradient(to left,#f97316,#b91c1c);
            color:#f9fafb;
        }
    </style>
</head>
<body>
    <div class="cover">
        <!-- background layer -->
        <div class="art"></div>
        <div class="gradient-overlay"></div>

        <div class="content">
            <!-- top strip -->
            <div class="top-strip">REVISED EDITION</div>

            <!-- title area -->
            <div class="title-block">
                <div class="subtitle-top">Hands-On Programming Guide</div>
                <h1 class="main-title">
                    PYTHON
                    <span>CRASH COURSE</span>
                </h1>
                <p class="tagline">
                    Learn <span>modern Python</span> with practical tasks and real-world examples.
                </p>
            </div>

            <!-- bottom area -->
            <div class="bottom-area">
                <div class="edition">FIRST EDITION</div>
                <div class="divider"></div>

                <div class="series">Advanced Programming · Project Oriented</div>

                <div class="author-block">
                    <div class="author-text">
                        <div class="author-label">Author</div>
                        <div class="author-name">Vignesh G</div>
                    </div>
                    <!-- you can replace this circle with your own photo using <img> -->
                    <div class="author-photo">
                        <span>👨‍💻</span>
                    </div>
                </div>

                <div class="code-badge">PY · FULL STACK</div>
            </div>
        </div>
    </div>
</body>
</html>

```

## OUTPUT:
<img width="453" height="656" alt="Screenshot 2025-11-27 113911" src="https://github.com/user-attachments/assets/d4bfa428-8e54-4879-adc4-4d246a222217" />


## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.

## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
