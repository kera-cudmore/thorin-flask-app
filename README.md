# Thorin & Co

![Thorin Responsive Site Image](documentation/thorin-responsive.png)

![GitHub last commit](https://img.shields.io/github/last-commit/kera-cudmore/thorin-flask-app?style=for-the-badge)
![GitHub contributors](https://img.shields.io/github/contributors/kera-cudmore/thorin-flask-app?color=yellow&style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/kera-cudmore/thorin-flask-app?color=orange&style=for-the-badge)
![GitHub top language](https://img.shields.io/github/languages/top/kera-cudmore/thorin-flask-app?style=for-the-badge)

Thorin Flask App was created as part of a flask walkthough project on the Code Institutes Level 5 Diploma in Web Application Development.

[Visit the deployed site.](https://web-production-4cc5.up.railway.app/)

---

## User Stories

* I want to be able to find out more information about Thorin and his Company.
* I want to be able to contact the Company.
* I want to be able to read some interesting articles relating to the Company.
* I want to be able to see any job positions within the Company.

- - -

## Design

This site uses the bootstrap clean blog template, this was chosen so that students could concentrate on using Flask and Jinja templating.
- - -

## Features

### General Features of the site

Each page of the site features a:

* Favicon

  ![Favicon image](documentation/favicon.png)

* Navbar (including responsive mobile navigation which utilises a hamburger menu)

  ![Navbar image](documentation/navbar.png)

  ![Mobile Navbar image](documentation/navbar-mobile.png)

* Footer

![Footer image](documentation/footer.png)

### Future Implementations

In a future implementation I would like to add further information to the site, such as battle stats etc for each member of the company. I would also like to improve on the blog functionality, as currently there are only 4 articles on the home page.

### Accessibility

I have been mindful during coding to ensure that the website is as accessible friendly as possible. This has been have achieved by:

* Using semantic HTML.
* Using descriptive alt attributes on images on the site.
* Providing information for screen readers where there are icons used and no text.
* Ensuring that there is a sufficient colour contrast throughout the site.

- - -

## Technologies Used

### Languages Used

* HTML
* CSS
* JavaScript
* Python3

### Frameworks, Libraries & Programs Used

* [Git](https://git-scm.com/) - For version control.

* [Github](https://github.com/) - To save and store the files for the website.

* [Shields.io](https://shields.io/) To add badges to the README.

* [Flask](https://flask.palletsprojects.com/en/2.1.x/) Version 2.2.2

* [Jinja](https://jinja.palletsprojects.com/en/3.1.x/) - A templating language

* [Bootstrap Clean Blog Template](https://startbootstrap.com/theme/clean-blog) Version 5.0.10

* [Font Awesome](https://fontawesome.com/) Version 6.2.0
- - -

## Deployment & Local Development

### Deployment

This project was initially deployed using heroku, before being redeployed using railway.


<details>
<summary>Expand for Railway Deployment Instructions</summary>
Since completing my diploma and due to Heroku removing their free tier in November 2022, I have migrated the deployment of this site to use railway.app. You can find instructions on how to migrate your app from Heroku to Railway in my [article here](https://www.codu.co/articles/migrating-your-heroku-app-to-railway-vf9p3kid).

Note that you will also need to create a runtime.txt in your environment which contains the version of python you are using. You can find this out by typing python --version in the terminal, and entering the result into the runtime.txt folder like so:

`Python -3.10.5`
</details>

<details>
<summary>Expand for Heroku Deployment Instructions</summary>

The site is deployed using Heroku. To deploy to Heroku:

1. To successfully deploy on Heroku we first need to create some files: a requirements.txt file and a Procfile.

2. The requirements.txt file contains all the applications and dependencies that are required to run the app. To create the requirements.txt file run the following command in the terminal:

    ```bash
    pip3 freeze --local > requirements.txt
    ```

3. The Procfile tells Heroku which files run the app and how to run it. To create the Procfile run the following command in the terminal:

    ```bash
    echo web: python app.py > Procfile
    ```

    NOTE: The Procfile uses a capital P and doesn't have a file extension on the end.

4. If the Procfile has been created correctly it will have the Heroku logo next to it. It is also important to check the Procfile contents, as sometimes on creation a blank line will be added at the end of the file. This can sometimes cause problems when deploying to Heroku, so if the file contains a blank line at the end, delete this and save the file. Make sure to save both these files and then add, commit and push them to GitHub.

5. Login (or sign up) to [Heroku.com](https://www.heroku.com).

6. Click the new button and then click create new app.

7. You will then be asked to give your app a name (these must be unique) and select a region. Once these are completed click create app.

8. You will now need to connect the Heroku app to the GitHub repository for the site. Select GitHub in the deployment section, find the correct repository for the project and then click connect.

9. Once the repository is connected, you will need to provide Heroku some config variables it needs to build the app. Click on the settings tab and then click reveal config vars button. You will now need to add the environment key/value variables that were used in the env.py file:

    | KEY | VALUE |
    | :-- | :-- |
    | IP | 0.0.0.0 |
    | PORT | 5000 |
    | SECRET_KEY| YOUR_SECRET_KEY* |

    *Denotes a value that is specific to your app.

10. You're now ready to click the enable automatic deploys and create button. Heroku will start building the app.

11. Click open app at the top of the screen and the Thorin application should now open in a new tab.
</details>

### Local Development

#### How to Fork

To fork the repository:

1. Log in (or sign up) to Github.
2. Go to the repository for this project, [Thorin Flask App Repo](https://github.com/kera-cudmore/thorin-flask-app).
3. Click the Fork button in the top right corner.

#### How to Clone

To clone the repository:

1. Log in (or sign up) to GitHub.
2. Go to the repository for this project, [Thorin Flask App Repo](https://github.com/kera-cudmore/thorin-flask-app).
3. Click on the code button, select whether you would like to clone with HTTPS, SSH or GitHub CLI and copy the link shown.
4. Open the terminal in your code editor and change the current working directory to the location you want to use for the cloned directory.
5. Type 'git clone' into the terminal and then paste the link you copied in step 3. Press enter.

- - -

## Testing

Testing was carried out throughout the build of the project. Please see the [testing file](TESTING.md) for more information.

- - -

## Credits

* Code Institute modules on Flask.

### Media

* [Image of Thorin & Company](https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/fadc668e-5f6a-4648-9d27-e91eb6973da7/d5nay7b-9991c1db-0f4a-4f3f-a95a-0b53947a14f9.png?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcL2ZhZGM2NjhlLTVmNmEtNDY0OC05ZDI3LWU5MWViNjk3M2RhN1wvZDVuYXk3Yi05OTkxYzFkYi0wZjRhLTRmM2YtYTk1YS0wYjUzOTQ3YTE0ZjkucG5nIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmZpbGUuZG93bmxvYWQiXX0.eknvKAWOPVaW_j6s7cbG6EKi-TGwolEaaTetCmjNYUA) used for the page header image.

* [Company Bio Information](https://lotr.fandom.com/wiki/Thorin_and_Company) Was taken from the Lord of the Ring Fandom Page for Thorin & Company.
