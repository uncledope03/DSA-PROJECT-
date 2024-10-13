# DSA-PROJECT-   discription
Here’s the breakdown of each method, now including the data structure used:

 1. `Phonebook()`
- Function**: Constructor that initializes the GUI components for the phonebook application.
- **Data Structure Used**: `ArrayList<Contact>` named `contacts`, which stores all contact objects in the application.
- **Purpose**: Sets up the main frame, text fields, buttons, and tabs for different operations (Add, View/Search, Update/Delete). This method also configures the layout and adds event listeners for user interactions.
  
 2. `createAddPanel()`
- **Function**: Creates a panel for adding contacts with text fields for entering contact information.
- **Data Structure Used**: `ArrayList<Contact>` (indirectly used when contacts are added).
- **Purpose**: Allows the user to input a contact's name and phone number and provides an "Add Contact" button to add the contact to the phonebook.

### 3. `createViewPanel(JScrollPane scrollPane)`
- **Function**: Sets up the panel for viewing and searching contacts.
- **Data Structure Used**: `ArrayList<Contact>` (used to display contacts in the list).
- **Purpose**: Displays all contacts in a scrollable list and provides search functionality through a text field and a search button. The user can also click a "View Contacts" button to refresh and display all contacts.

### 4. `createUpdatePanel()`
- **Function**: Creates a panel for updating and deleting contacts.
- **Data Structure Used**: `ArrayList<Contact>` (used when a contact is selected to be deleted or updated).
- **Purpose**: Provides the user with buttons to delete or update a selected contact. This panel is used to modify or remove existing contacts.

### 5. `createButton(String text, Color color)`
- **Function**: Helper method to create a button with specified text, color, and style.
- **Data Structure Used**: N/A (not related to data storage).
- **Purpose**: Centralizes the button creation process, making it easy to set consistent styling and properties for buttons across the application.

### 6. `actionPerformed(ActionEvent e)`
- **Function**: Handles actions for buttons throughout the application, specifically the "Add Contact" button in this case.
- **Data Structure Used**: `ArrayList<Contact>` (used to store the new contact).
- **Purpose**: Adds a new contact to the `contacts` list when the "Add Contact" button is clicked. It checks if the contact name and phone are not empty and if they’re unique before adding. Displays success or error messages based on the operation result.

### 7. `isUniqueContact(String name, String phone)`
- **Function**: Checks if the provided name or phone number is unique within the `contacts` list.
- **Data Structure Used**: `ArrayList<Contact>` (used to iterate and check each contact for duplicates).
- **Purpose**: Prevents duplicate contacts by verifying that no contact with the same name or phone number exists in the list.

### 8. `viewContacts()`
- **Function**: Sorts the contacts alphabetically and updates the display list.
- **Data Structure Used**: `ArrayList<Contact>` (used to sort and view contacts).
- **Purpose**: Refreshes the contact list view, ensuring that contacts are displayed in a sorted order for easier viewing.

### 9. `searchContacts()`
- **Function**: Searches for contacts that match the text in the `searchField` and filters the display list accordingly.
- **Data Structure Used**: `ArrayList<Contact>` (used to iterate through each contact to match the search query).
- **Purpose**: Allows the user to search for contacts by name or phone. It updates the display to show only the contacts that match the search query. If no matches are found, a message is displayed.

### 10. `deleteContact()`
- **Function**: Deletes the selected contact from the `contacts` list after user confirmation.
- **Data Structure Used**: `ArrayList<Contact>` (used to remove a contact by index).
- **Purpose**: Removes a contact from the phonebook. Prompts the user for confirmation before deleting and then removes the contact if confirmed, displaying a success message.

### 11. `updateContact()`
- **Function**: Allows the user to update the name or phone number of the selected contact.
- **Data Structure Used**: `ArrayList<Contact>` (used to update the selected contact).
- **Purpose**: Retrieves the current values for the selected contact and prompts the user to input new values. The contact is updated if the new information is unique, and a message confirms the successful update.

### 12. `sortContacts()`
- **Function**: Sorts the `contacts` list alphabetically by contact name.
- **Data Structure Used**: `ArrayList<Contact>` (used to sort contacts in place).
- **Purpose**: Keeps the contacts organized by name. This helps with displaying and searching for contacts, as an alphabetically sorted list is generally easier to navigate.

### 13. `main(String[] args)`
- **Function**: Entry point of the application.
- **Data Structure Used**: N/A (initializes the application).
- **Purpose**: Starts the phonebook application by invoking the constructor and initializing the GUI.

### 14. `Contact` (Inner Class)
- **Attributes**: `name` and `phone` (both `String` types).
- **Methods**:
  - `getName()`: Returns the name of the contact.
  - `setName(String name)`: Updates the contact’s name.
  - `getPhone()`: Returns the phone number of the contact.
  - `setPhone(String phone)`: Updates the contact’s phone number.
  - `toString()`: Returns a formatted string containing the contact’s name and phone number.
- **Data Structure Used**: N/A (represents a contact object).
- **Purpose**: Represents a contact with a name and phone number. This class provides basic getter and setter methods for managing contact data and a `toString` method for easy display within the list.


[DSA Group Project 2.pdf](https://github.com/user-attachments/files/17357132/DSA.Group.Project.2.pdf)


  
