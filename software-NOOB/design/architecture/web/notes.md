https://boom.co/blogs/complex-react-architecture/

#### Software Architecture
:=> the study of the broader structure, organization, and patterns
of a development project-primarily the ones that impact developer 
productivity overtime

###### Goals
- design software that fits the contraints and required uses 
- will be constantly changing throughout its lifetime 

## Server-Side Rendering (SSR) ::: basics

#### client-side Rendering
- renders app to HTML in the user's browser
- load index.html from server, loads JS bundle from server, runs bundle 
, displays app, loads data 
- less strain on the server, but generally slower user experience 

#### server-side rendering 
- renders app to HTML on the server 
- runs JS bundle, loads data, creates HTML document, sends to client side 
- faster user experience and better for SEO, but more strain on server 

#### State Management
- how an application handles the data needs of its components, with regards
to loading, storing, persisting and sharing the data.
- differents sizes of state 
    1. small state : useState, Context 
    2. medium state : Recoil 
    3. Large state : Redux, MobX 



