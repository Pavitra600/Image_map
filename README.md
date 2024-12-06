# Ex04 Places Around Me
# Date: 4/11/2024
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
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Map Example</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: salmon;
            text-align: center;
            color: #333;
        }

        h1 {
            margin-top: 20px;
            font-size: 2rem;
        }

        .image-container {
            margin: 20px auto;
            display: inline-block;
            border: 2px solid antiquewhite;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            overflow: hidden;
        }

        .image-map {
            max-width: 100%;
            height: auto;
            display: block;
            border-radius: 8px;
        }

        area {
            cursor: pointer; /* Change cursor to pointer on hover */
        }
    </style>
</head>
<body>
    <h1>IMAGE MAP</h1>
    <div class="image-container">
        <img src="Screenshot 2024-10-20 170337.png" usemap="#image-map" class="image-map">
    </div>

    <map name="image-map">
        <!-- MedPlus Link -->
        <area target="_self" alt="MedPlus" title="MedPlus" href="https://www.medplusmart.com/" coords="1392,716,1658,784" shape="rect">
        <!-- Service Centre Link -->
        <area target="_self" alt="Service Centre" title="Service Centre" href="https://www.servicecentreinfo.com/" coords="620,382,922,479" shape="rect">
        <!-- Furniture Shop Link -->
        <area target="_self" alt="Furniture Shop" title="Furniture Shop" href="https://www.ikea.com/" coords="702,605,1012,683" shape="rect">
        <!-- Home Link -->
        <area target="_self" alt="Home" title="Home" href="https://www.example.com/home" coords="1205,188,1287,288" shape="rect">
    </map>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Service Center</title>
    <style>
        /* General body styling */
        body {
            background-color: burlywood;
            text-align: center;
            font-family: 'Times New Roman', Times, serif;
            font-size: 1rem;
            margin: 0;
            padding: 0;
            color: #4a4a4a;
        }

        h1 {
            background-color: brown;
            color: #fff;
            padding: 20px 0;
            margin: 0;
            font-size: 2.5rem;
        }
        /* Image styling */
        img {
            width: 300px;
            height: 300px;
            border-radius: 15px;
            border: 3px solid #8b5e34;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            margin-top: 20px;
        }

        /* Paragraph styling */
        p {
            font-size: 1.1rem;
            line-height: 1.8;
            width: 80%;
            max-width: 900px;
            margin: 20px auto;
            text-align: justify;
            color: black;
        }

       

        /* Small screen adjustments */
        @media (max-width: 768px) {
            img {
                width: 70%;
                height: auto;
            }

            p {
                font-size: 1rem;
                width: 90%;
            }
        }
    </style>
</head>
<body>
    <h1>SERVICE CENTER</h1>
    <img src="colleagues-working-together-call-center-office_23-2149256147.avif" alt="Service Center">
    <p>
        A service center is a place that offers products or services to users, or a commercial establishment that provides repairs and replacement parts.
        A service center is a hub of support and expertise, dedicated to helping customers maintain and repair their products. Whether it's electronics, appliances, or vehicles, service centers are staffed with skilled technicians who provide thorough diagnostics and reliable solutions. With a focus on customer satisfaction, these centers offer not just repairs but also guidance on product care and maintenance. The welcoming atmosphere and commitment to quality service ensure that clients leave feeling confident in their choices, knowing they have access to the help they need to keep their items in top condition.
    </p>
   
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Medical Store</title>
    <style>
        /* General body styling */
        body {
            background-color: lightpink;
            text-align: center;
            font-family: 'Times New Roman', Times, serif;
            margin: 0;
            padding: 0;
            color: #4a4a4a;
        }
        h1 {
            background-color: hotpink;
            color: #fff;
            padding: 20px 0;
            margin: 0;
            font-size: 2.5rem;
        }
        /* Image styling */
        img {
            width: 80%;
            max-width: 600px;
            border-radius: 15px;
            border: 3px solid #6a4b36;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            margin: 20px auto;
            display: block;
        }

        /* Paragraph styling */
        .content {
            margin: 20px auto;
            width: 80%;
            max-width: 800px;
            line-height: 1.8;
            text-align: justify;
            color: black;
            font-size: 1.2rem;
        }

      
    </style>
</head>
<body>
    <h1>MEDPLUS</h1>
    <img src="medplus.jpg" alt="Medical Store Image">
    <div class="content">
        <p>
            A medical store, also known as a pharmacy or chemist shop, is a retail establishment that sells medicinal products and healthcare supplies. Pharmacies also provide counseling on prescription and over-the-counter drugs, health problems, and wellness issues.
        </p>
        <p>
            A medical shop is a vital resource in the community, providing essential health supplies and medications to support well-being. Stocked with a range of products, from over-the-counter remedies to prescription medications, these shops serve as a first point of contact for health concerns. 
        </p>
    </div>
    
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Furniture Shop</title>
    <style>
        /* General body styling */
        body {
            background-color: plum;
            text-align: center;
            font-family: 'Georgia', serif;
            margin: 0;
            padding: 0;
            color: #4a4a4a;
        }

        /* Header section */
        h1 {
            background-color: palevioletred ;
            color: #fff;
            padding: 20px 0;
            margin: 0;
            font-size: 2.5rem;
        }

        /* Image styling */
        img {
            width: 300px;
            height: 300px;
            margin: 20px auto;
            display: block;
            border-radius: 15px;
            border: 3px solid #8b5e34;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }

        /* Paragraph styling */
        p {
            font-size: 1.2rem;
            line-height: 1.8;
            margin: 20px auto;
            width: 80%;
            max-width: 800px;
            text-align: justify;
            color:black
        }

       
    </style>
</head>
<body>
    <h1>FURNITURE SHOP</h1>
    <img src="furniture.jpg" alt="Furniture">
    <p>
        A furniture shop, also known as a furniture retailer or furniture store, is a business that sells furniture and related accessories. Furniture shops typically sell a variety of furniture, including beds, tables, bookcases, wardrobes, couches, sofas, and chairs. A furniture shop is a treasure trove of possibilities, showcasing a diverse array of styles, colors, and designs to transform any space.
    </p>
   
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home</title>
    <style>
        /* General body styling */
        body {
            font-family: 'Times New Roman', Times, serif;
            font-size: 1.2rem;
            background-color: turquoise;
            margin: 0;
            padding: 0;
            text-align: center;
            color: black;
        }

        /* Header section */
        h1 {
            background-color: darkolivegreen;
            color: #fff;
            padding: 20px 0;
            margin: 0;
            font-size: 2.5rem;
        }

        /* Image styling */
        img {
            width: 300px;
            height: 300px;
            border-radius: 15px;
            border: 3px solid #8b5e34;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
            margin-top: 20px;
        }

        /* Paragraph styling */
        p {
            margin: 20px auto;
            width: 80%;
            max-width: 800px;
            line-height: 1.8;
            text-align: justify;
            color: black;
        }

      
    </style>
</head>
<body>
    <h1>MY HOME</h1>
    <img src="simple-home-design-Warm-grey-exteriors.png " alt="Home Image">
    <p>
        Home is more than just a physical space; it’s a sanctuary filled with memories, warmth, and comfort.
        It’s where laughter echoes through the halls and where the simplest moments, like sharing a meal or curling up with a book, 
        become cherished rituals. Each room tells a story, reflecting the personalities of those who inhabit it, making home a unique
        tapestry of love and belonging. Whether it's a cozy apartment or a sprawling house, home is the heart's true refuge.
    </p>
    
</body>
</html>




# OUTPUT
![image](https://github.com/user-attachments/assets/67d48fdf-8c0d-455b-ba1b-0945bf9677c8)
![image](https://github.com/user-attachments/assets/1952725c-6c55-468c-bc61-365bb454fa96)
![image](https://github.com/user-attachments/assets/3a33298f-8a84-4cfe-8ee0-01ef095c9a0e)
![image](https://github.com/user-attachments/assets/821b5347-efba-4fab-80ba-f9811b22f2af)
![image](https://github.com/user-attachments/assets/02da92c4-ec54-44b4-b112-238c0ca518b5)





# RESULT
The program for implementing image maps using HTML is executed successfully.
