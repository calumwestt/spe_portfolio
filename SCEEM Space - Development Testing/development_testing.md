# SCEEM Space
### Software Product Engineering - Portfolio
##### Jason Park, Sungjin Kang, William Nafack, Calum West
----------------------------------------------------------

## Development Testing

The key concept of this project was to manage data dynamically. This means that the data needs to be stored accurately when being manipulated by administrators. There are several different things we have to do to ensure this is the case. We have developed test cases for the service layer of our system and have made sure to utilise the database where possible.

### Back-end testing

With this project we found it difficult to fix problems when they arose, resulting in a redesign of the system. In this redesign we made sure to create several new test cases in order to prevent previous problems. We did this by utilising 'SpringBootTest' and 'Test'. The test cases we created ensured that all the requirements given by the client for the website application were met.

This table contains some of our test cases:

| Web App Requirements                                  | Test Cases                                                  |
| ----------------------------------------------------- | ----------------------------------------------------------- |
| Detection of duplicate member id's and location names | DUPLICATE_REGISTER_MEMBER_NAME, DUPLICATE_REGISTER_LOCATION |
| Detection of duplicate member email addresses         | DUPLICATE_REGISTER_MEMBER_EMAIL_ADDRESS                     |
| Allocation and deallocation                           | ALLOCATION, DE_ALLOCATION                                   |
| Registration of member and location                   | REGISTER_MEMBER, REGISTER_LOCATION                          |
| Detection of lack of desks                            | OVERFLOW_MAXIMUM_DESKS_AVAILABLE                            |

Before connecting to AWS RDS, we first used the H2 database which is an in-memory database. We did this to test the functions we have made work correctly. After setting AWS RDS, we connected it to the project and then would see the tables in the database functions were working correctly.

### Front-end testing

The front end is tested visually, by checking if the web page is showing as expected. Once we know that everything is correct, we can map the front end and the back end together. The mapping of the back end variables successfully conform with the front end properties.

It is challenging to test front end components of the application due to there not being many effective tools to do so. To overcome this we are making sure that when visually testing the front end, we are doing so methodically and recording any errors we find to make it easier to create a list of fixes that need to be made.
