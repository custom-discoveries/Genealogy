## Genealogy
This is a Tigergraph schema example of the Rockefeller family tree, starting with William Avery Rockefeller Sr.
The gsql queries are an example of how to add edges dynamically to a skeleton graph.
## Install and Run
### Install
To install this TigerGraph demo, clone this repository at a terminal command prompt: 
- \>git clone https://github.com/custom-discoveries/Genealogy.git
### Run Cheetah in Cloned Directory:
-  cd Genealogy
-  Genealogy\> Cheetah
    - (See Cheetah [README.md](https://github.com/custom-discoveries/Cheetah/blob/main/README.md) for installation and setup of Cheetah)
### In TigerGraph GraphStudio:
Run the query scripts in the following order in TigerGraph GraphStudio Write Queries:
  1. setRelationships - to setup basic relationships - Mother, Father, Son, Daughter
  2. setAdvancedRealationships - to setup more advanced relationships - Uncle, Aunt, GrandFather, GrandMother
  3. setRoles_subquery - This will add a list to the Person object in which a relationship has been assigend to the person
  4. resetRelationships - This script will delete ALL relationships except for the primary relationship hasParent/hasChild
  5. deleteParentChildRelationship - This script will delete the primary relationship hasParent / hasChild from the graph
  6. displayPersonsByName - Allows you to either lookup a person by their ID or by their First or Lastname
  7. displayPersonByRole - Allows you to find all Persons that have been taged with a relationships
