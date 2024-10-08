# DSA-PROJECT-


 INSERT CONTACT
 
public void insertContact(String name, String phone) {
    contacts.add(new Contact(name, phone));
}


 Search Contact
public Contact searchContact(String name) {
    for (Contact contact : contacts) {
        if (contact.getName().equalsIgnoreCase(name)) {
            return contact;
        }
    }
    return null; // Not found
}


Display All Contacts

public void displayContacts() {
    for (Contact contact : contacts) {
        System.out.println(contact);
    }
}

 Delete Contact

 public boolean deleteContact(String name) {
    Iterator<Contact> iterator = contacts.iterator();
    while (iterator.hasNext()) {
        Contact contact = iterator.next();
        if (contact.getName().equalsIgnoreCase(name)) {
            iterator.remove();
            return true; // Successfully deleted
        }
    }
    return false; // Not found
}


Update Contact

public boolean updateContact(String name, String newPhone) {
    for (Contact contact : contacts) {
        if (contact.getName().equalsIgnoreCase(name)) {
            contact.setPhone(newPhone);
            return true; // Successfully updated
        }
    }
    return false; // Not found
}

