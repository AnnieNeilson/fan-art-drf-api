# Fan Art API
Fan Art is a content sharing website for people who like to create artwork based on their favourite things.

This repository is the backend of the application using the Django REST Framework(DRF) holding the API database for the front end part of the application.

## Links
[The deployed API](https://fan-art-drf-api.herokuapp.com/)  
[The deployed site](https://fan-art.herokuapp.com/)  
[The Frontend repository](https://github.com/AnnieNeilson/fan-art)  
[My Github Project](https://github.com/users/AnnieNeilson/projects/4)

## Contents
- [Database Schema](#database-schema)
- [Technologies Used](#technologies-used)
    * [Languages](#languages)
    * [Frameworks, Libraries and Programs](#frameworks-libraries-and-programs)
- [Testing](#testing)
    * [Validator Testing](#validator-testing)
    * [Manual Testing](#manual-testing)
        * [Testing User Stories](#testing-user-stories)
        * [Url Path Testing](#url-path-testing)
- [Deployment](#deployment)
- [Credits](#credits)
  
## Database Schema
I created this Entity relationship diagram to help visualise the backend of this project

![Entity relationship diagram](./images/EntityRelatonshipDiagram.PNG)

## Technologies Used

### Languages
* Python  
-- The Django REST Framework base language

### Frameworks, Libraries and Programs
* Cloudinary
-- storage of images
* Pillow  
-- image processing capabilities
* Git  
-- For version control, committing and pushing to Github
* Github  
-- For storing the repository, files and images pushed from Gitpod
* Gitpod  
-- IDE used to code project
* Heroku  
-- Used to deploy the application
* Django Rest Auth
* PostgreSQL
* Cors headers


## Testing

### Validator Testing

I ran the files from this project through an online PEP8 validator and recorded the results in the following table:
![PEP8 Validator results](./images/pep8-validator-testing.PNG)

### Manual Testing
#### Testing User Stories

1. Admin Profiles List: As an admin, I would like to be able to view all profiles so that I can moderate them for inappropriate content.
* I visited the [admin site](https://fan-art-drf-api.herokuapp.com/admin/) and logged in with the admin credentials. From there I followed the link to Profiles, I'm presented with a list of profiles. I can visit any profile and see the details of their profile

2. User Sign In: As a web server I would like to be able to authenticate user credentials so that users can sign in and use the site.
* I signed in successfully as a user

3. User Sign Up: As a web server I can POST a user to the database so that new users can register for the site.
* I signed up as a new user and noted that the API had a record of this new account

4. User Sign Out: As a web server I can POST an empty object so that users can logout of the site.
* I was able to successfully sign out.

5. GET Profile: As a web server I can get a specific user profile so that it can be displayed to the user.
* Using the user id of the profile I wanted to see, I was able to retrieve the correct profile data

6. Update Profile: As a web server I can PUT an updated profile in the database so that users can update their profiles.
* Whilst signed in I updated my username, the database updated the information

7. GET Filtered Posts: As a web server I can retrieve a list of filtered posts so that the user can search for specific posts.
* I used the search function available in the deployed site, it was fully functional

8. GET Filtered Posts: As a web server I can retrieve a list of filtered profiles so that users can search for specific profiles.
* I used the search function available in the deployed site, it was fully functional

9. Get Post List: As a web server I can retrieve a list of posts so that they can be displayed to the users.
* Using the url ending with '/posts/' I can see all posts listed. 

10. GET Post: As a web server I can retrieve a specific post so that it can be displayed to the user
* Using a url with the post id I retrieved the post data, using the link on the deployed site works as well

11. DELETE Post: As a web server I can delete a specific post so that the user can delete their post
* When accessing the delete function from the deployed site the instance is removed from the database

12. PUT Post: As a web server I can PUT an updated post so that the user can edit their post
* When accessing the edit function from the deployed site the instance is updated in the database

13. POST Post: As a web server I can PUT a new post so that the user can create a new post
* When submitting a new post to the deployed site the instance is created in the database

14. POST Comment: As a web server I can POST a comment to a post so that the user can create a comment
* When submitting a new comment to the deployed site the instance is created in the database

15. PUT Comment: As a web server I can PUT an updated comment so that users can update their comments
* When accessing the edit function from the deployed site the instance is updated in the database

16. DELETE Comment: As a web server I can delete a specific so that users can delete comments
* When accessing the delete function from the deployed site the instance is removed from the database

17. GET Comment List: As a web server I can retrieve the comments on a specific post so that it can be displayed to the user
* Using the url ending with '/comments/' I can see all comments listed. 

18. GET Sorted and Filtered Posts: As a web server I can retrieve a sorted and filtered posts so that popular items can be shown to the users
* When accessing the search feature on the deployed site the filtered results are displayed with more recent posts first

19. GET Sorted and Filtered Posts: As a web server I can retrieve sorted and filtered profiles so that they can be displayed to the user
* When accessing the search feature on the deployed site the filtered results, posts by users matching the search term, are displayed with more recent posts first

#### Url Path Testing

I tested all the url paths and recorded the results in the following table:
![url path results](./images/urlpathchecks.PNG)

## Deployment

## Prepare API for deployment to Heroku

## Deployment to Heroku

## Credits

I referenced [this README.md file](https://github.com/Mrst12/pp5-backend-drf-appy-families/blob/main/README.md) for help with the structure and layout of this README.md file.

## Acknowledgements