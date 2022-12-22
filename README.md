# Code Refactor Starter Code

## Description

This is a primarily a routine maintenance on the Horiseon business website.

## Usage

Marketing Website for Website services



The following list of file created and madified for this project:

Pull Requests:



[alt text](assets/images/)

HTML File:
<!DOCTYPE html>
<html lang="en-us">
<!-- items that need to be corrected -->
<!-- change title on website tab from website to Horiseon -->
<!-- when you hover on an image, display a description -->
<!-- make sure all hyperlinks work -->
<!-- consolidate/simplify style sheet -->
<!-- add description to images if image does not display -->
<!-- rename repo -->
<!-- make images load quicker will not be done during this maint session -->
<!-- document flow and css code -->
<!-- make sure all code is pretty print lined up-->
<!-- professional readme--> 

<!-- overall flow-->
<!-- three hyperlinks at top right of page-->
<!-- links scroll down this images that are already displayed on website. ie. don't go to tabbed page-->
<head>
    <meta charset="UTF-8" />
    <!-- title changed to promote name brand -->
    <title> Horiseon For All Your Social Media Needs </title>
    <link rel="stylesheet" href="./assets/css/style.css">
    
</head>

<body>
    <div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <!-- three hyperlinks at top of page on right side -->
        <!--add assessibility text for each image hover code in css?-->
        
        <!-- code to support links at top of page -->
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization" atl="Search ENgine Optimization">Search Engine Optimiztion</a>
                </li>
                <li>
                    <a href="#online-reputation-management" atl="Online Reputation Management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing" atl="Social Media Marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>

    <!-- display left side of screen in this order: background(hero), -->
    <!-- search-engine-optimization,online-reputation-management, social-media-marketing -->

    <!-- background image -->
    <!-- no inline style. all selectors in style.css file-->
    <div class="hero"></div>
    <div class="content">
<!-- fixed broken link by adding id -->
        <div id="search-engine-optimization" class="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg" alt="Search Engine Optimization" 
                 class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
            </p>
        </div>
        <div id="online-reputation-management" class="online-reputation-management">
            <img src="./assets/images/online-reputation-management.jpg" atl="Online Reputation Management" 
                 class="float-right" />
            <h2>Online Reputation Management</h2>
            <p>
                The web is full of opinions, and some of these can be negative. Social media allows anyone with an internet connection to say whatever they want about your business. Online Reputation Management gives you the control over what potential customers see when they search for your business.
            </p>
        </div>
        <div id="social-media-marketing" class="social-media-marketing">
            <img src="./assets/images/social-media-marketing.jpg" atl="Social Media Marketing 
                 class="float-left" />
            <h2>Social Media Marketing</h2>
            <p>
                Social media continues to have a sizable influence on buying habits. Social media marketing helps you determine which platforms are suited to your brand, using analytics to find the right markets and increase your lead generation.
            </p>
        </div>
    </div>
    <!-- right side of screen display: lead-generation, brand awareness, benefit cost -->
    <div class="benefits">
        <div class="benefit-lead">
            <h3>Lead Generation</h3>
            <img src="./assets/images/lead-generation.png" atl ="Lead Generation"/>
            <p>
                Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.
            </p>
        </div>
        <div class="benefit-brand">
            <h3>Brand Awareness</h3>
            <img src="./assets/images/brand-awareness.png"atl="Brand Awareness"/>
            <p>
                Users find your business through paid and organic searches, increasing the search ranking and visibility for your business.
            </p>
        </div>
        <div class="benefit-cost">
            <h3>Cost Management</h3>
            <img src="./assets/images/cost-management.png" atl=" Cost Management"></img>
            <p>
                As the search ranking for your business increases, your advertising costs decrease, and you no longer need to advertise your page.
            </p>
        </div>
    </div>
    <div class="footer">
        <h2>Made with ❤️️ by Horiseon</h2>
        <p>
            &copy; 2019 Horiseon Social Solution Services, Inc.
        </p>
    </div>
</body>

</html>

Style.CSS file:
/* use entire screen real estate for display */
/* the "*" means all box sizing and all borders for box */
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}

body {
    background-color: #d9dcd6;
}

.header {
    padding: 20px;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    background-color: #2a607c;
    color: #ffffff;
}
/* three tabs at top of screen displayed hortizonally */
.header h1 {
    display: inline-block;
    font-size: 48px;
}
/* selector for span statement in html */
.header h1 .seo {
    color: #d9dcd6;
}

.header div {
    padding-top: 15px;
    margin-right: 20px;
    float: right;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    font-size: 20px;
}

.header div ul {
    list-style-type: none;
}

.header div ul li {
    display: inline-block;
    margin-left: 25px;
}

a {
    color: #ffffff;
    text-decoration: none;
}

p {
    font-size: 16px;
}
/* main background image for website */
.hero {
    height: 800px;
    width: 100%;
    margin-bottom: 25px;
    background-image: url("../images/digital-marketing-meeting.jpg");
    background-size: cover;
    background-position: center;
}

.float-left {
    float: left;
    margin-right: 25px;
}

.float-right {
    float: right;
    margin-left: 25px;
}

.content {
    width: 75%;
    display: inline-block;
    margin-left: 20px;
}

.benefits {
    margin-right: 20px;
    padding: 20px;
    clear: both;
    float: right;
    width: 20%;
    height: 100%;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #2589bd;
}
/* these next three statements can be combined */

.benefit-lead + .benefit-brand + .benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}

/*
.benefit-lead {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}
*/
/* these next three selectors can be comnbined */
.benefit-lead h3 + .benefit-brand h3 + .benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
}
/*
.benefit-lead h3 {
    margin-bottom: 10px; 
    text-align: center; 
}

.benefit-brand h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
}
*/
/* combining the next three class selectors doesn't display first image */
/*
.benefit-lead img + .benefit-brand img + .benefit-cost img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}
*/

.benefit-lead img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-brand img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-cost img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

/* the next three class selectors are be combined */
.search-engine-optimization , .online-reputation-management , .social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
/* 
.online-reputation-management {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}

.social-media-marketing {
    margin-bottom: 20px;
    padding: 50px;
    height: 300px;
    font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    background-color: #0072bb;
    color: #ffffff;
}
*/
/* the next three class selectors can be combined */
.search-engine-optimization img  {
    max-height: 200px;
}

.online-reputation-management img {
    max-height: 200px;
}

.social-media-marketing img {
    max-height: 200px;
}

/* the next three statements can be combined */
.search-engine-optimization h2 + .online-reputation-management h2 + .social-media-marketing h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

/*
.search-engine-optimization h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.online-reputation-management h2 {
    margin-bottom: 20px;
    font-size: 36px;
}

.social-media-marketing h2 {
    margin-bottom: 20px;
    font-size: 36px;
}
*/
.footer {
    padding: 30px;
    clear: both;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    text-align: center;
}

.footer h2 {
    font-size: 20px;
}




To add a screenshot, create an assets/images folder in your repository and upload your screenshot to it. Then, using the relative filepath, add it to your README using the following syntax:


## Credits

Various TA, classmates and information gathered from website searches provided the knowledge and guidance for the maintenance of the website.

Extensive tutorials from the GT Web Developer BootCamp and Code Academy were used.

List your collaborators, if any, with links to their GitHub profiles.


## License
A MIT License was used for this project.
