# Instructions: Working with HTML and CSS
1. **Note:** The page design has been re-organised into sections using `<section>` tag:
    - `<section id="mainsection">` updated to `<div class = "container">`
    - `<section id="projectsection">` (newly included)
2. Look for `projectsection` and update the cards within as follows:
    ```HTML
    <!-- Project card #1 -->
    <div class="projectcard">
        <a href="#">
            <img src="img/web-design.jpg" alt="Add a description here">
            <!-- Project name -->
            <h4>Community Web Portal Design</h4>
            <p class="scope">Web Page Design</p>
            <p><span>UI/UX</span><span>HTML</span><span>CSS</span></p>
        </a>
    </div>
    <!-- Project card #2 -->
    <div class="projectcard">
        <a href="#">
            <img src="img/mobile-app.jpg" alt="Add a description here">
            <!-- Project name -->
            <h4>Expense Calculator Web App</h4>
            <p class="scope">JavaScript Development</p>
            <p><span>User Interaction</span><span>Application Logic</span></p>
        </a>
    </div>
    <!-- Project card #3 -->
    <div class="projectcard">
        <a href="#">
            <img src="img/data-tracking.jpg" alt="Add a description here">
            <!-- Project name -->
            <h4>Enrollment Tracker</h4>
            <p class="scope">Database Design</p>
            <p><span>SQL</span><span>Data Analysis</span></p>
        </a>
    </div>
    <!-- Project card #4 -->
    <div class="projectcard">
        <a href="#">
            <img src="img/chess.jpg" alt="Add a description here">
            <!-- Project name -->
            <h4>Chess Game</h4>
            <p class="scope">Java</p>
            <p><span>Game Development</span></p>
        </a>
    </div>
    <!-- Project card #5 -->
    <div class="projectcard">
        <a href="#">
            <img src="img/fitness-tracking.jpg" alt="Add a description here">
            <!-- Project name -->
            <h4>Fitness Tracker</h4>
            <p class="scope">App Development</p>
            <p><span>SwiftUI</span><span>Swift Programming</span></p>
        </a>
    </div>
    <!-- Project card #6 -->
    <div class="projectcard">
        <a href="#">
            <img src="img/photography.jpg" alt="Add a description here">
            <!-- Project name -->
            <h4>SG Arts Award</h4>
            <p class="scope">Photography</p>
            <p><span>Creative</span><span>Competition</span></p>
        </a>
    </div>
    ```
3. Update the styles to apply the changes for ***projectsection***
    Add the following styles for projectsection.
    ```css
    /* Start of styling projectsection */
    /* ******************************* */
    /* Set projectsection's style*/
    #projectsection {
        width: 80%;
        margin: auto;
        height: 100dvh;
    }
    /* Set the showcasecontainer to list the projects, repeated in equal columns of 3s per fractional unit */
    .showcasecontainer {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        grid-gap: 24px;
    }
    /* Set the card background to white */
    .projectcard {
        font-size: small;
        background-color: white;
        border-bottom-left-radius: 10px;
        border-bottom-right-radius: 10px;
        padding-bottom: 24px;
    }
    /* Set the projectsection grid container's content with a left padding */
    .projectcard h4, .projectcard p {
        padding-left: 16px;
    }
    /* Set the image in the project card */
    .projectcard img {
        display: block;
        border-top-left-radius: 10px;
        border-top-right-radius: 10px;
        margin-bottom: 10px;
        width: 100%;
        height: 180px;
        background-size: cover;
        background-position-x: center; 
        background-position-y: center;
        background-repeat: no-repeat;  
        background-image: url("img/imgplaceholder.png");
        text-indent: -9999px; /* remove or comment out text indent if all images are available */
    }
    /* Set the projectcard title's style (set the text to be uppercase) */
    .projectcard .scope {
        text-transform: uppercase;
        padding-top: 8px;
        padding-bottom: 8px;
    }
    /* Set mouseover effect for project card */
    .projectcard:hover {
        transition: 0.45s ease-out;
        transform: scale(1.05);
    }
    .projectcard a {
        text-decoration: none;
        color: gray;
        transform: scale(1.0);
    }
    .projectcard span{
        display: inline;
        align-content: space-between;
        border-radius: 6px;
        margin-right: 4px;
        background-color: lightseagreen;
        padding: 5px 10px;
        color: white;
    }
    /* ***************************** */
    /* End of styling projectsection */
    ```
4. Add within `projectsection` the below for users to go to the top of the page:
    ```HTML
    <div class="top">
        <a href="#top">&#x25B2; Back to Top</a>
    </div>
    ```
5. To style the contents for **Back to Top**, include the following styles:
    ```css
    /* Start of styling miscellaneous elements */
    /* *************************************** */
    .top{
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .top a{
        margin-top: 20px;
        text-decoration: none;
        color: lightseagreen;
        font-size: small;
    }
    /* ************************************* */
    /* End of styling miscellaneous elements */
    ```