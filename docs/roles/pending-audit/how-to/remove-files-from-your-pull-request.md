When you submit a pull request, make sure that you don't include any unrelated files. This will help your reviewers focus on your changes.

### If you've added a file to a PR by mistake, try this to remove it:

The following command will give you the commit hash for the last commit on the upstream/gh-pages branch

`git rev-parse upstream/gh-pages`

This next command reverts the file(s) that you want:

`git checkout <THE COMMIT HASH FROM PREVIOUS STEP> -- <PATH OF THE FILE(S) YOU WANT TO REMOVE (separated by a space)>`

> Here's an example:
> `git checkout 9af8d8c7f34cb4dfda49cd8372236f8b8bd1ea65 -- pages/wins/wins.html _sass/components/_wins-page.scss`

Since you only need the first seven digits of the commit hash (aka SHA value), you can also type this: 

> `git checkout 9af8d8c -- pages/wins/wins.html _sass/components/_wins-page.scss`
