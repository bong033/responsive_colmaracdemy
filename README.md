## Setting up my Git Repository

1. Instruction to set up my local folder to point to Github

    ```BASH

    echo "# colmaracademy" >> README.md  
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin https://github.com/bong033/colmaracademy.git
    git remote -v
    git push -u origin main

    ```

2. In the event remote url is set incorrectly

    ```BASH

    git remote set-url origin https://github.com/bong033/colmaracademy.git
    git remote -v
    git push -u origin main

    ```

3.  Important Note on css specificity:

    .   Universal selector (*) targets every element (regardless tag, class, ID)
    .   If pseudo class :root is used, :root takes priority over html
        .   When applied, font size of 5px takes priority over that of html
    .   Here, html selector takes priority as root element over universal selector

    * {
        margin: 0;
        padding: 0;
    }

    /* :root{ font-size: 5px; } */

    html, body {
        box-sizing: border-box;
        font-family: "Lato", sans-serif;
        font-size: 16px;
    }

