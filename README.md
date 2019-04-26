Exercise: 09. Defining objects with prototypes
Tasks

1. Create a constructor function for a prototype called Discussion. Create a new instance of the Discussion prototype using the constructor function and assign it to a variable named discussion.
2. The renderComment function is currently declared and assigned to a variable. Attach it to the Discussion prototype as a method instead. The renderComment function is called twice directly. Adjust this so that the renderComment method on the Discussion instance is used instead.
3. The updateCommentCount is currently declared and assigned to a variable. Attach it to the Discussion prototype as a method instead. The updateCommentCount function is called once directly. Adjust this so that the updateCommentCount method on the Discussion instance is used instead.
4. There is a prototype AddCommentForm, which represents the "Add comment" text input and button. Within the handleCommentSubmitted method of this prototype, make use of the renderComment method of discussion so that the message taken from the input is added to the DOM.
5. Add a new method to the Discussion prototype named renderInitialComments. Use this new method to create the two initial comments and set the initial comment count already in the script. Use this in the method to refer to the current discussion instead of using the variable reference discussion. Don't forget to add the method call for the discussion instance afterwards!
6. Add a parameter initialComments to the Discussion constructor function. Assign this parameter to a property comments in the Discussion prototype and use the property in renderInitialComments instead of referencing the global variable  comments. Now the Discussion constructor function can be used to create any number of initial comments. Create the discussion object with an array of just one comment.
7. The updateCommentCount method is set to always use 2 as the number of comments. Adjust the method so that it uses the length of the comments property of discussion to set the text for the number of comments instead of the hard-coded value 2.
8. The comment count is not updated when a new comment is added. Create a new method on the Discussion prototype called addComment that accepts one parameter  newComment. Use this new method instead of renderComment in the  AddCommentForm.handleCommentSubmitted method. Implement the new addComment method so that it will:
  - 1.- Add the comment to the comments array of the Discussion.
  - 2.- Render the comment in page.
  - 3.- Update the comment count displayed on the page.
