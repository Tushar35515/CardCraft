How would your tables and apis change for the following scenarios. What tables and api endpoints would you add? Which tables and api endpoints would need to be updated?


Q1:- If a user can create and edit stages for a particular board. For example instead of Open > In Progress > Done if they want the stages of their task board to be Read > Working > Reviewing > Completed

Answer:- Tables: You may need to add a "Stages" table to store stage configurations for each user's board.
         API Endpoints: Add API endpoints for: Creating and editing stages for a board and Retrieving and updating stage configurations.
         Update: You may need to update the "Boards" table to include a reference to the user's selected stage configuration

   
Q2:- If users can comment on tasks

Answer:- Tables: Add a "Comments" table to store task comments, linking each comment to the corresponding task.
         API Endpoints: Add API endpoints for: Creating, editing, and deleting comments on tasks and Retrieving comments for a specific task.


Q3:- How will you do error handling?

Answer:- I have added some checks in a code to handle errors like what if column and board is empty.
         Also we can make log errors on the server for debugging and monitoring purposes.
         We can write Test cases for different scenarios to which will help in handling the errors.
