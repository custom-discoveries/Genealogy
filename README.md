## Genealogy
This is a Tigergraph schema example of the Rockefeller fiamly tree, starting with William Avery Rockefeller Sr.
The gsql queries are an example of how to add edges dynamically to a skeleton graph.

Run the query scripts in the following order:
  1. setRelationships - to setup basic relationships - Mother, Father, Son, Daughter
  2. setAdvancedRealationships - to setup more advanced relationships - Uncle, Aunt, GrandFather, GrandMother
  3. setRoles_subquery - This will add a list to the Person object in which a relationship has been assigend to the person
  4. resetRelationships - This script will delete ALL relationships except for the primary relationship hasParent/hasChild
  5. deleteParentChildRelationship - This script will delete the primary relationship hasParent / hasChild from the graph
  6. displayPersonsByName - Allows you to either lookup a person by their ID or by their First or Lastname
  7. displayPersonByRole - Allows you to find all Persons that have been taged with a relationships
