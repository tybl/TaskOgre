# Requirements

## Views

### Task List

* A task is displayed as a summary with a checkbox to the left
* When the checkbox is clicked, the summary text is greyed out 
* When the summary is clicked, the task details are displayed
* How are the tasks ordered?

### Task Details

| Attribute     | Type      | Multiplicity | Origin    | Mutability |
|---------------|-----------|--------------|-----------|------------|
| Creation ts   | date/time | 1            | Generated | Immutable  |
| Completion ts | date/time | 0-1          | Generated | Toggled    |
| Summary text  | String    | 1            | Supplied  | Can edit   |
| Details/Notes | String    | 0-1          | Supplied  | Can edit   |
| Tags          | String    | 0-\*         | Supplied  | Can edit   |
| Waiting For   | Reference | 0-\*         | Sup/Gen   | Can edit   |
| Required By   | Reference | 0-\*         | Sup/Gen   | Can edit   |

* Change history

### Tag Details

* Name

### Ideas to flush out:

* The URL structure
** hostname is the login page
** hostname/UUID is the user's main task view
** hostname/UUID/listname is the user's specified/configured list of tasks
** I want to have another UUID as the task identifier, but I'm not sure how to differentiate it from the list name...
