# Classy Django REST Framework.

## What is this?

[Django REST framework](http://www.django-rest-framework.org) is a powerful and flexible toolkit that makes it easy to build Web APIs. It provides class based generic API views and serializers. We've taken all the attributes and methods that every view/serializer defines or inherits, and flattened all that information onto one comprehensive page per class. This project is heavily based on [Classy Class-Based Views](http://ccbv.co.uk) and was developed by [Vinta Software Studio](http://www.vinta.com.br).

## Dependencies
* Python 2.7
* s3cmd (For deploy)

## Building

`pip install -r requirements.txt`

`fab build`

The first build will take a while.

To run locally:

`fab runserver`

## Deployment

create a .env file with the content:

```
AWS_BUCKET_NAME=''
AWS_ACCESS_KEY_ID=''
AWS_SECRET_ACCESS_KEY=''
```

Make sure you have built it as instructed above and deploy via

`fab deploy`

## Help
If you have any questions or need help, please send an email to: contact@vinta.com.br
