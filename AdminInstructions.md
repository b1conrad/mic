# Admin Instructions

## Becoming an admin

To become an admin of this system request the right to commit to this repository.

Start by becoming familiar with the single page which everyone can see: [index.html](https://b1conrad.github.io/mic/).
To learn, open the page itself and the source code in two windows side-by-side.
Notice the one-to-one correspondence between things on [the page](https://b1conrad.github.io/mic/) 
and things in [the source code](https://github.com/b1conrad/mic/blob/main/index.html).
Your changes to the source code will correspond to changes on the page.

All admin functions will be done by editing this page in the repo and committing your changes.

## Maintaing the list of instruments

### To add an instrument to an existing category:
1. Take a picture of the instrument, named by the instrument name (make sure it is unique)
2. Upload it (as a `.jpg` file) in the corresponding folder (from the "Add file" dropdown select "Upload files")
3. Locate the category in the source code
4. Determine where to place the new instrument in the list
5. Add a new line of code at that spot, precisely mimicking another instrument, changing the category-slash-picture-file twice and the picture name twice
6. Commit your changes
7. Wait a few minutes and check the page to ensure that your new instrument is showing correctly in the desired place

### To check-out an instrument
1. A student appears with a screenshot of the instrument they want
2. Check their student ID card to ensure that it is them and that they are eligible
3. If the instrument is available, give it to them
4. Write down the instrument name, student ID, and expected return date (as you did before this system was in place)
5. After the student has gone, edit the source code file (locate the line for the instrument and replace `<button onclick="alert` with `<button disabled onclick="alert`)
6. Commit your changes
7. After a few minutes, visit the page to ensure that the "Check out" button for that instrument is grayed-out

### To check-in an instrument
1. The student appears to return the instrument
2. Thank them and handle the return as you did before this system was in place
3. After the student has gone, edit the source code file (locate the line for the instrument and remove the word "disabled" from the button)
4. Commit your changes
5. After a few minutes, visit the page to ensure that the "Check out" button for that instrument operates

### To add a new instrument category
1. Decide where it goes wrt the other categories
2. Prepare to edit the source code
3. Choose a name for the category (shown here as "Percussion")
4. Choose a new lower-case letter for the category (shown here as "p")
5. At that point in the source code, add these HTML tags (replacing the category name and letter throughout):

```
\<h2>Percussion\</h2>
\<input class="p" type="checkbox">Instruments
\<div class="p">
\</div>
```

6. Near the top of the source code, locate lines like the one shown below (within a `<style>` tag) and insert a new line, changing the new category letter from "p" to the new category letter, in two places:

```
input.p[type="checkbox"]:checked ~ div.p {display: block;}
```

7. Commit your changes
8. After a few minutes, visit the page to ensure that the new category appears
9. After you have inserted a new instrument in it, check that the "Instruments" checkbox works

