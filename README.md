# Rails Partials, Helper Methods, & Routing Practice

## Part 1: Conceptual questions
1. What's the benefit of using partials, and why are locals a supplmental feature Rails give us?
2. In an MVC framework, where should the logic associated to database queries be placed? (M, V, or C?) 
3. Order M, V, and C starting with where we should place most App logic to where we should place least App logic.    
* What type of logic/responsibility is permissible in each?

## Part 2: Boat Rental App
* In the previous challenge you built a form that allows the manager to record a new rental, associating an existing boat and a new customer
* Boats have many Customers through Rentals
* Customers have many boats through Rentals

### PART 2A - Build some helper methods
* Using a partial with locals, build a simplistic index page for Boats that displays a list of Rental info for each Boat
* Build a view helper method that displays the rental date in the format: "Day_of_Week, Month Day, Year" ("Monday, January 3, 2019") and use this on the Boat index page
* Build a custom query method that returns only the rentals taking place in the future (after current datetime) and use this on the Boat index page
* BONUS: Add server validations and display them in form

### PART 2B - Build a rental index and baot show page with a nested resource
* Build a boat show page that lists all the associated rentals along with an associated nested resource ('/boats/:id/rentals')
* Link to each boat show page from the rentals index page