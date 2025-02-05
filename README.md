# Firebase Non-Existent Field Access Error
This repository demonstrates a common yet easily overlooked error in Firebase when accessing document fields that might not exist.  The `bug.js` file shows the problematic code that attempts to access a non-existent field without proper error handling. The `bugSolution.js` file provides a corrected version that includes proper null checks or default values.

## How to Reproduce
1. Clone the repository.
2. Install the Firebase SDK: `npm install firebase`
3. Configure your Firebase project.
4. Run `bug.js`.  You should see an error.
5. Run `bugSolution.js`.  This should run without errors, even if the field doesn't exist.

## Solution
Always check for the existence of fields before accessing them to prevent unexpected errors and improve your application's robustness. Use optional chaining or default values to safely access potentially missing fields.