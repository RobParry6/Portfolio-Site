<p>"Read Me a Story" was an app that was produced collaboratively over a 10 day period using technologies and tech stacks that were unfamilar to us.</p>

<p>The premise for "Read Me a Story" is that family members can remotely upload readings of children's stories to cloud based services and then a parent can then playback the recordings to the child. Readings can be either an individual story which can be uploaded on its own or recordings can be added to existing stories to create a 'book' with chapters, which will display all the recordings under the one title.</p>

<p>The front end of the project was written in typescript and made use of the svelte framework to build the project. Svelte kit was used to provide routing to the app and firebase was used in order to handle the autentication side of things.</p>

<p>The back end was comprised of a RESTful Api wirtten in Python and used the flask framework in order to create the API. Firebase's cloud services were used to store the audio files and Firebase's realtime database was used to store all the information about the families, stories and users.</p>

<p> A link to the front end repository can be found here: <a href="https://github.com/yangalexyangg/fe-read-me-a-story">Read Me A Story - Front End</a></p>

<p> A link to the back end repository can be found here: <a href="https://github.com/yangalexyangg/be-read-me-a-story">Read Me A Story - Back End</a></p>

<style>
    p {
        margin: auto;
        margin-bottom: 16px;
        width: 60%;
    }
    </style>