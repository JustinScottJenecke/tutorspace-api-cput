# tutorspace-api-cput
Simple Spring-Boot API for Tutorspace

##API entry point:
    /ts/api/v1/post
    
    returns String as a soft guide to different uri endpoints

## Post entity endpoints:

### Get all Posts
    URI:
    /ts/api/v1/post/all

    Details:
    Returns List of all Posts in database

### Create Post
    URI:
    /ts/api/v1/post/create

    Details:
    Request body must contain a Post object
    (int student no, String firstName, lastName, email, phone, institution, major, subject)

    Object Id is generated by Database

### Read single Post
    URI:
    /ts/api/v1/post/read/{id}

    Details:
    Returns a Post object by given Id
    Path parameter must be of type Integer

### Update Post
    URI:
    /ts/api/v1/post/update

    Details:
    Request body must contain a Post object
    Updates existing Post with data in body of sent Post
    
    Id of existing Post must be included in request body

### Delete Post by ID
    URI:
    /ts/api/v1/post/delete/{id}

    Details:
    Deltes an existing Post object by given Id
    Path parameter must be of type Integer


    