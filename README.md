![CICD Webooks (1)](https://user-images.githubusercontent.com/20936398/230953538-305cc363-74b7-4093-bfd2-4b43a7d9b9ff.png)


## CI/CD Hooks Now in Assembla

Assembla users can now seamlessly link their Travis CI account with Assembla and view and manage their builds in the Assembla user interface. In this tutorial, I’ll be walking you through it A-Z. 

## Let's get started

Let’s first go to your repository section in Assembla: 

![Screenshot 2023-04-10 at 8 20 17 AM](https://user-images.githubusercontent.com/20936398/230939604-35ea81a9-09c4-4058-9721-75b37cac5b0f.png)

>Look for the repository you're looking for.

In that repository in Assembla make sure you have your `.travis.yml` file in it. Here's an example one I did: 

![Screenshot 2023-04-10 at 8 31 23 AM](https://user-images.githubusercontent.com/20936398/230939876-014b9442-3934-4632-b739-72dbc30d7dbc.png)

>YAML File

Now you're gonna want to look for the "Builds" tab in Assembla: 

![Screenshot 2023-04-10 at 8 14 00 AM](https://user-images.githubusercontent.com/20936398/230940010-dbe611d1-4276-460a-9e52-60b2ea176ed5.png)

>Builds Tab

Once you click on the “Builds” tab, you should see something similar to this:

![Screenshot 2023-04-10 at 8 13 50 AM](https://user-images.githubusercontent.com/20936398/230940092-d7739912-0622-4c60-9e5e-7b16ad1921ed.png)

## API Token Creation 

Press enable, you’ll want to generate your API token through the CLI using the command `travis token –-pro` (make sure you have the Travis gem installed.):

<img width="373" alt="Screenshot 2023-04-10 at 8 56 36 AM" src="https://user-images.githubusercontent.com/20936398/230940816-80792609-6d38-431a-a09a-aefd6e7cf7a2.png">

>Generating the API token through the CLI

Now you’ll want to sign into Travis by going to [app.travis-ci.com], and clicking “Sign-in” then clicking “Assembla":

![Screenshot 2023-04-10 at 8 44 54 AM](https://user-images.githubusercontent.com/20936398/230940987-0fe32cd0-7488-436d-92fb-65f8d15a0a2f.png)

>Sign in page

Once you’re signed in via Assembla, you can now try starting your build! It should look like this when it’s starting in the Builds tab once your build has passed:

![Screenshot 2023-04-10 at 8 47 57 AM](https://user-images.githubusercontent.com/20936398/230941209-bd28ed76-8cde-46b5-b4a8-0b736a24ebc6.png)

>Passing build status in Assembla

Say if you start another build in Travis, and want to see the verbosity of the outputs, etc, you can certainly do that by going back to the Travis CI GUI:

![Screenshot 2023-04-10 at 8 16 08 AM](https://user-images.githubusercontent.com/20936398/230941434-831f6f4e-f925-4b83-ad00-c6bb512588b0.png)

>Travis GUI

## Conclusion 

There you go, now you know how you can manage and access your Travis CI builds directly through Assembla using the CI/CD hooks with just simply using an API key.

As always if you have any questions, any questions at all, please email me at [montana@travis-ci.org](mailto:montana@travis-ci.org).

Happy building and Assemblaing! 

