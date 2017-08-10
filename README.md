# Google Moderator Clone
#### Colin Beard, Danielle Pankey, Eshawn Karim, Nick Khoury, Ling Li

This app will allow users to create a series, which contains user comments and questions. 

## App run cycle

Upon entering the site, the user will be prompted to login, and then will have access to all series and also the ability to create their own series. 

If a user owns a series and logs into the application and enters that series, they will get the admin view, which contains data that can be edited about the series itself. If not, they are a guest which cannot edit any of the series information but can post comments and statements about the series that can be upvoted or downvoted by other guests.

Series will contain statements from other users or the creator about a particular topic, and each statement will have a vote value. Voting will make this value go up or down based on the feedback received, and the highest value will be displayed at the top.

### Models, Views, and Collections
##### AllSeries Collection
This is a collection of ```series``` collections.
##### Series Collection
This is an actual series collection which contains a title, a description, the author, and a bunch of ```statement``` models.
##### Statement Model
This model contains a comment or question from any registered user along with a score and two buttons that will increment and decrement the score. The statement with the highest score in a series will be displayed first.

### Admin GUI
Contains fields for a s screen foradmins. This viewwill include:a.A title fieldb.A Descriptionfieldc.A field forownersd.A cancel andsubmissionbutton