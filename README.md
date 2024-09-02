1. Data Structures and Initialization
Struct Definitions:
store: Holds the cost of travel and intermediate nodes (for path reconstruction).
initialdata: Stores initial costs for direct flights.
Class Definitions:
datamodule: Manages city data and cost declaration.
bellmanfordalgorithm: Implements the Bellman-Ford algorithm for finding the shortest path between cities.
filehandlingmodule: Handles file operations for user login, account creation, and ticket information.
inputmodule: Manages user input for city selection and account login.
outputmodule: Displays available cities, ticket prices, and detailed ticket information.
2. Class datamodule:
Constructor Initialization:

Initializes an array of city names.
costdeclaration() Method:

Sets up a 2D array (arr) with travel costs between cities, where infinity represents no direct flight.
Copies this array into travel and ini structures, where travel will be updated by the Bellman-Ford algorithm.
3. Class bellmanfordalgorithm:
Constructor Initialization:

Sets the number of cities (N).
algorithmic_implementation() Method:

Implements the Bellman-Ford algorithm to compute the shortest paths between all pairs of cities.
Updates the travel structure with the shortest path costs and paths.
4. Class filehandlingmodule:
log_in() Method:

Reads user credentials from a file (login.txt) and validates login attempts.
createaccount() Method:

Appends new user credentials to the file (login.txt).
ticket() Method:

Writes ticket information to a file (ticket.txt).
5. Class inputmodule:
user_input() Method:

Prompts the user to enter the source and destination cities.
login() Method:

Allows users to either log in or create a new account.
Repeatedly prompts until successful login.
noofpassenger() Method:

Asks for the number of passengers.
6. Class outputmodule:
initial() Method:

Displays the main menu with options to list cities or book tickets.
list_cities() Method:

Lists all available cities.
ticket() Method:

Displays ticket details including total price, source, destination, and number of passengers.
passengerdetailedticket() Method:

Shows detailed information for each passenger.
display_price() Method:

Computes and displays the price of traveling between source and destination cities.
Provides options for direct or indirect routes based on user input.
7. Main Function:
Initialization:

Creates instances of datamodule and bellmanfordalgorithm classes.
Initializes cost data and runs the Bellman-Ford algorithm.
User Interaction:

Calls the inputmodule for user login and choice.
Displays the main menu and handles user choices (listing cities or booking tickets).
Execution Flow:
Initialization:

City data and travel costs are set up.
Bellman-Ford algorithm computes the shortest paths.
User Login/Account Creation:

Users can log in or create an account.
Main Menu Interaction:

Users can list cities or book tickets.
Ticket booking involves checking flight prices, choosing routes, and entering passenger details.
File Handling:

Ticket details are saved to a file, and user credentials are managed.
