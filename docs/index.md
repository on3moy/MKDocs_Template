# MkDocs Template
A Mkdocs Template using third-party customization such as **Material**

<img src='img/trex.png' width=300/>

## Customize Mkdocs Theme
If you want to quickly customize your theme, I suggest you start with built in themes!  
[Choosing Your Theme](https://www.mkdocs.org/user-guide/choosing-your-theme/)


## Customize Mkdocs Theme with Material (Third Party Source)
If you like more capabilities for customization, try using **Material**.   
`pip install mkdocs-material`     
[Material Installation](https://squidfunk.github.io/mkdocs-material/getting-started/)  
[Material Theme Setup](https://squidfunk.github.io/mkdocs-material/customization/?h=theme#setup-and-theme-structure)

!!! warning Note
    Before going through customization, ensure you know whether you want to use built in themes from MkDocs or Third Party.  
    - Built-in themes from Mkdocs is easier to work with and modify.  
    - Third-party themes such as Materials requires you use their documentation only for customization. 

## Creating and Deploying to Github Pages
1. First you can create your page and develop everything you need to without doing anything in GIT.  
    - `mkdocs new project_name`
2. Test out the changes and content.
    - `mkdocs serve`
3. When you are ready to publish and made all your changes.
    - mkdocs build will create a new folder called **site**. This folder will be referenced when publishing.
    - `mkdocs build`
4. Publish your folder/code to your github 
    - Requires a few steps, GIT installation, an IDE, GitHub account, etc.  
    - `mkdocs gh-deploy`
        - This will automatically create git pages and create a link
5. Any further changes you want to add, you will use `mkdocs build` then `mkdocs gh-deploy` for the changes.  

BAM! Thats it assuming there were no issues with your Github account.  
Author: Moy Patel 🦖