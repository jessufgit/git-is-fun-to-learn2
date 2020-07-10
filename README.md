# git-is-fun-to-learn2 (Pushing and Pulling)

In the first part of this series, you created a repository locally and connected it to your Git Hub account. It's now time to learn about pushes and pulls to git hub.

The repository you have locally on your computer can push information up to, or receive information back from, the same repository that is hosted on Git Hub. It's helpful to have the changes you make locally separate from the Git Hub repo. This way, you can be certain that your code is behaving exactly as you expect before you share it with the world. Another side benefit is that you will always have a fresh copy to retrieve from Git Hub should something disastrous happen to your local copy - well - as long as you have been pushing your changes up to origin/master.

In this activity, you will practice pushing up you make locally to the repository on Git Hub. You will also make changes directly on Git Hub and pull them down to your local version of the repository.

### Push

In the terminal, navigate into the repository you created in the first part of the series.

Then on your desktop open the folder that contains the README with the your favorite movie line. Open the README and make a change to the document in some way. You could add another favorite line, add the character's name or even just make some styling changes. Save the document.

Next in the terminal, type git status. You should notice that the document you just edited is highlighted in red. In the terminal, add the README to the staging area. Then you will commit a message to describe the change you just made. Replace the word second commit with a more descriptive message. This will be important as you grow as a developer for locating certain changes you have made in the future. Finally, you will push these changes to the repository you have on Git Hub. This will make the copy of this repository on Git Hub a mirror of what you have locally.

    $ git add README.md
    $ git commit -m "second commit"
    $ git push
    
Checkout the updated copy on Git Hub by refreshing your page.

### Pull

Now we are going to reverse the process. You are going to make a change to the git hub repository and pull down those changes locally.

On your Git Hub page, you should already be on the README page of your repo with the your favorite movie line. Make a change to the README in some way. Click on the pencil in the right hand corner to do this. You could add another favorite line, add the character's name or even just make some styling changes. Save the document by clicking the commit changes button at the bottom of the page.

Next in the terminal, type git status. You should see the following:

    Your branch is up to date with 'origin/master'.
    nothing to commit, working tree clean

This is because your local copy does not know that you've made changes to the copy on Git Hub. In the terminal now run the following:

    $ git pull
    
You will get a message that may read something like...

    remote: Enumerating objects: 5, done.
    remote: Counting objects: 100% (5/5), done.
    remote: Compressing objects: 100% (2/2), done.
    remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
    Unpacking objects: 100% (3/3), done.
    
and then something towards the bottom with the name of the document you modified and some + signs.
If you now open the repository folder on your desktop and examine the README file - you should see that it has been changed to reflect the change you made on Git Hub.

Congratulations! You have learned how to both push to and pull from your Git Hub repository.


