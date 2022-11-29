# Development

### Link to Deployed Website
https://crazyrhino1300.github.io/try2/ 

### Goal and Value of the Application
As a classical musician, I've alwyas found it a pitty how underappreciated classical music can be. As such, the goal of this
application is to allow users to gain better insight into the different composers and eras that exist in the classical musical world.
Users are also able to click on each composer to learn more about their specific works and biography. This application has value in that
it allows for the preservation of classical music knowledge and culture. IF I had more time, I would definitely add more filters to be more 
explicit in the different epochs that different composers might fall into. I would also present a wider array of composers, but the amoutn of 
JSON manipulation was a barrier.

### Usability Principles Considered
- At the top of the gallery, I display what filters are in effect so that the user knows the state of the application
- On the left, i have the aggregator move along with the user's scrolling so that the user knows what composers he or she has already
  liked.
- for each composers' biography, I allow an easily collapsible offcanvas that allows users to easily transition between browing the gallery
  and learning about a specific composer
- There is a clear hierarchy between all of the headings, composer names, and the liked composers.

### Organization of Components
- The page is divided into left and right; 
    - on the left, there's a component that shows the average age of the composers liked, as well as a list of all of the liked composers
    - on the right, there are clickable cards with clickable photos that allow users to learn more. users can also click the heart or the X 
      to add or remove a composer from their favorites list. 

### How Data is Passed Down Through Components
- Most data relating to the gallery, sorting, and filtering of composers remains in the app component. 
- Each of the composers has their own card, which is its own component. each json object is mapped into a card component
- within each card component, the composers information is funneled into an offcanvas component as well in order to create the informational
  component.
### How the User Triggers State Changes
- the user can click the drop-downs for the different filters
- the user can click the sort button to sort
- the user can click the reset button to reset all sorting and filters
- the user can add and subtract from their favorite composers.

