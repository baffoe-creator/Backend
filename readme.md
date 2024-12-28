Bike Rental Shop

This Bash script creates a command-line interface for a simple bike rental shop. Users can rent bikes, return rented bikes, and view available bikes. The script interacts with a PostgreSQL database to store bike and customer information.

How it Works

The script defines a function MAIN_MENU that displays a menu to the user and prompts them to choose an action (rent a bike, return a bike, or exit).
Based on the user's selection, the script calls the corresponding function:
RENT_MENU: This function retrieves available bikes from the database and displays them to the user. It then prompts the user to select a bike and handles the rental process, including checking bike availability, registering new customers, and updating the database.
RETURN_MENU: This function allows users to return rented bikes. It prompts the user for their phone number, retrieves their rental information from the database, and updates the bike's availability in the database.
The script uses psql commands to interact with the PostgreSQL database.
Requirements

PostgreSQL database
psql command-line tool
Instructions

Save the script as a file (e.g., bike_rental.sh).
Make the script executable: chmod +x bike_rental.sh
Run the script: ./bike_rental.sh
Note: This is a basic example and can be extended to include additional features such as tracking rental duration, calculating fees, and managing different bike types.