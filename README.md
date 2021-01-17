# COVID19-Voice-Contact-Tracing
Hack the North 2020++ Submission using Voiceflow and Dropbase API

## Inspiration
The fundamental inspiration of the project lies in the newly adopted premise of COVID-19 questionnaires being presented to any medical location that one visits. Many other appointment-based businesses have also adopted this strategy; sometimes in the form of emails and other times via mobile. I thought about all of this information being collected and yet contact-tracing seems to remain a couple weeks behind in reaching peak efficacy. 

Hence I thought about utilizing this large amount of data to try and improve contact-tracing by creating a service that pushes all information onto one large database. This will result in not only a more seamless delivery in the form of voice assistants, but also provide an easy to navigate environment for professionals to see where the virus has traveled throughout a community

## What it does
The *COVID-19 Voice-Aided Contact Tracing* app works on two key premises:
1.  processing answers to COVID-19 related questions that help determine who is at high risk of being exposed to the virus
2. Uploading the data to a relational database for easy access when needed and thereby reducing the need of having multiple different platforms that slows down contact-tracing tremendously

## How I built it
The entire application's foundation is based upon the powerful tools provided by Voiceflow and the beta version (albeit very effective) of Dropbase's new RESTful API. The fundamental workflow was created using Voiceflow's Alexa-based (Google Assistant is perfectly viable too) speaking response tiles while JSON data structures were created using the update SET logic. API integration was done using the dedicated custom panels that allow for RESTful interfaces like Dropbase's new offering to be utilized fully while also keeping course with standard HTTP protocols.

The database itself was based on PostgreSQL with the help of PostgREST documentation that aided in understanding the fundamentals effectively. Dropbase was used to provide an ease of database creation with one-click initialization of filler datasets obtained from custom tags created in Mockaroo.

## Challenges I ran into
The primary challenge I ran into was trying to navigate different environments throughout the entire project. The modular nature of Voiceflow made it difficult for me to find subsequent areas that I explicitly-coded using JSON-types while the entire PostgreSQL platform was a new skill that I learned through utilizing a beta-version of the REST API from Dropbase (the API token was not available for many hackers, initially causing difficulty but the staff helped us overcome it by administering fixes on a case-by-case basis )

## Accomplishments that I'm proud of
The single largest accomplishment that I am proud of throughout this entire weekend is my ability to learn new frameworks through documentation and one hour introductory workshops. Prior to this hackathon I had never heard of either Voiceflow or Dropbase but both technologies caught my attention almost immediately and to my surprise fit with each other almost seamlessly, allowing me to create a project that increased my horizons tremendously.

## What I learned
I learned the basics of **PostgreSQL** and spent a lot of time with **Voiceflow** which also taught me the basics of **Alexa Developer Tools** and how to utilize that to emulate an Alexa environment even without any real Alexa-enabled devices.

## What's next for COVID-19 Voice-Aided Contact Tracing
The next steps for this app is to expand itself into a modular element that can be hosted in various platforms ranging from apps to websites so that any place that asks such COVID-19 related questions to others can have an easily manageable database that can be used if the need for contact-tracing arises. A second development could incorporate NLP into the Voiceflow framework (they are currently working on it) so that a wider variety of answers can yield proper results.

Hopefully small businesses and clinics adopt this technology and see an increased level of safety and also time efficiency via the use of voice-assistants and open-source relational databases such as PostgreSQL
