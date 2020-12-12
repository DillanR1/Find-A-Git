# Find-A-Git
Git hub finder app built from the Traversy Media Udemy Course "React Front to Back"

Find-A-Git is a github user search tool that uses Axios and the github API.

# Deployed App Link
Be sure to read the instructions first, but if you'd rather dive in that's cool too!

   https://find-a-git.netlify.app/


# Instructions 
To use Find-A-git, simply type the username or the name of the user you would like to find. If you have a github account, try to find your own profile.
If not, no worries! Search for DillanR1, and then try searching dillan. Compare the results between the two search methods.


# Why this project is awesome | Implementation | Methodology 


Building Find-A-Git was a very necessary exercise, as it highlights several important tools that developers can implement to write cleaner code in React.

Learning to implement Axios for a small tool like Find-A-Git is ideal and is what is used to fetch requests from the github API.

Originally the app used hard coded values for the input fields in the app. Find-A-Git was then completely rebuilt and refactored from class based components 
to functional / stateless components.

Holy prop drilling batman! No Redux? No problem. While Redux may be the preferred option for larger applications, similar functionality was achieved using the Context API.
Through the Context API, "Use reducer" and "Use Context hook" were available.

NOTE: State was initially passed through the users component in the app and THEN passed through props.

It was mentioned in this tutorial that "Use Reducer" and "Use Context" could achieve a 
similar "Flux Pattern" to Redux. While flux patterns seem to be beyond the scope of this particular project, flux patterns seem like something worth investing some time in.
I did find an interesting article on flux patterns provided by freeCodeCamp. 

LINK: https://www.freecodecamp.org/news/an-introduction-to-the-flux-architectural-pattern-674ea74775c9/



APP.JS was refactored to use Async await on component did mount. This makes error handling easier, cleans up the code, and also allows other functions of the App to load while
awaiting the promise to be fulfilled. This is my current level of understanding with Async/Await in a nut shell, with excellent examples being provided by MDN. 

LINK: https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Asynchronous/Async_await



# Github API
There are a couple of interesting things to note about the github API.

The github API is said to only allow 50 requests per hour, unless an API key is used. I did not test this theory, but it seems like a reasonable assumption (to me at least)

Integrating the API key required the use of registering the Find-A-Git app as a "new O Auth app" on github, and entering the API key in the designated fields. 

# Thanks
Documenting my findings allows for reflection on what I have learned by building this project, but I also hope this information is able to help someone out!






