

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Profile Card</title>
</head>

<body>

    <h1 id="heading1">Student Profile</h1>

    <h2 class="name">Anamta</h2>

    <p class="message">Welcome to my student profile.</p>
    <p class="message">I am learning HTML and JavaScript.</p>

    <button id="colorButton">Change Color</button>

    <div id="box">
        This is my profile box.
    </div>

    <br><br>

    <a id="googleLink" href="https://www.google.com">
        Visit Google
    </a>


    <script>
         1. Use getElementById() to change the h1 text
        const heading = document.getElementById("heading1");
        heading.textContent = "My Student Profile";


        2. Use getElementsByClassName() to change student's name color to blue
        const studentName = document.getElementsByClassName("name");
        studentName[0].style.color = "blue";


         3. Use querySelectorAll() to change both paragraphs to green
        const messages = document.querySelectorAll(".message");

        messages.forEach(function(message) {
            message.style.color = "green";
        });


        4. Change body background color to lightgray
        document.body.style.backgroundColor = "lightgray";


         5. When button is clicked, change body background to lightblue
        const button = document.getElementById("colorButton");

        button.addEventListener("click", function() {
            document.body.style.backgroundColor = "lightblue";
        });


        // 6. Use getAttribute() to get the link href
        const link = document.getElementById("googleLink");

        const linkAddress = link.getAttribute("href");

        console.log(linkAddress);


        7. Use setAttribute() to open link in a new tab
        link.setAttribute("target", "_blank");


        8. Use classList.add() to add active to #box
        const box = document.getElementById("box");

        box.classList.add("active");


         9. Use classList.contains() to check active class
        const hasActiveClass = box.classList.contains("active");

        console.log(hasActiveClass);


         10. Use parentElement to print the box's parent
        console.log(box.parentElement);
    </script>

</body>
</html>
