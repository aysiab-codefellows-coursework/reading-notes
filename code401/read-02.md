# Reading Assignment 02\
*Read:*
- [MDN Node/Express Intro](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction)
- [npm docs](https://docs.npmjs.com/about-npm)
- [TDD article](https://www.agilealliance.org/glossary/tdd/#q=~(infinite~false~filters~(postType~(~'page~'post~'aa_book~'aa_event_session~'aa_experience_report~'aa_glossary~'aa_research_paper~'aa_video)~tags~(~'tdd))~searchTerm~'~sort~false~sortDirection~'asc~page~1))
- [GitHub Training Vid](https://www.youtube.com/watch?v=xSv_m3KhUO8&ab_channel=GitHubTraining%26Guides)



### Reading & Discussion 
1. What's the difference between a `PUT` and `PATCH`?
`PUT` allows for a *complete* replacement of a document only, where `PATCH` is used to make changes to an existing document. 
[Medium Article](https://medium.com/backticks-tildes/restful-api-design-put-vs-patch-4a061aa3ed0b#:~:text=HTTP%20PUT%20method%20only%20allows%20a%20complete%20replacement%20of%20a%20document.&text=HTTP%20resource.&text=A%20PATCH%20request%20on%20the,the%20resource%20%E2%80%94%20changing%20its%20properties.)


2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
- [Postman](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)
- [Nock](https://github.com/nock/nock)
- [Stoplight](https://stoplight.io/mocking/)

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

Swagger unsuccessful API call:
- 400 bad request
- 401 lacking authorization
- 404 not found 

APIDOC.js unsuccessful API call:
Truthfully, I'm confused about this even after vewing the documentaiton for it [here](https://apidocjs.com/deprecated.html).


4. Compare and contrast SOAP and ReST
ReST has an easier learning curve, is efficient and fast. ReST also requires HTTP but that makes it closer to web design philosophies. It is optimized for web. 

SOAP works better with large, enterprise level environments. It's standardise and has built in error handling. However, there is a bit more to learn (it heavily relies on XML over HTTP). SOAP has tighter security than ReST however. 
[Upwork Article](https://www.upwork.com/resources/soap-vs-rest-a-look-at-two-different-api-styles)

### Define
**Web Server:** is a combination of hardware and software that allow webpages to be hosted on the internet. It is a relationship of requests and responses between hardware and software to produce web applications and their routes. 
[MDN - Web Servers](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/What_is_a_web_server)

**Express:** is a popular Node framework, and provides the ability to write handlers for requests at different URL endpoints, integrate with a view port, and can request additional processing from middleware. 

**Routing:** is how a web application can access certain routes & endpoints and respond with the correct logic or data. 

**WRRC:** is an acronym for the *Web Request Reponse Cycle*. In brief, the WRRC starts when a user types in an url and presses enter. The browser then must make a request for the URL, and the router then routes the URL to the correct handlers for the request. The request then passes forward to the view port and renders the page. This gets send back to the browser for the user. 

[Code Academy on WRRC](https://www.codecademy.com/articles/request-response-cycle-static)