## Deploy again!

If you have made changes locally and you want to deploy on PythonAnywhere again, you can follow the instructions below after each of the changes:

### Commit, and push your code up to Github

First off, let's see what files have changed since we last deployed (run these commands locally, not on PythonAnywhere):

{% filename %}command-line{% endfilename %}
```
$ git status
```

Make sure you're in the `djangogirls` directory and let's tell `git` to include all the changes within this directory:

{% filename %}command-line{% endfilename %}
```
$ git add --all .
```

> __Note__ `--all` means that `git` will also recognize if you've deleted files (by default, it only recognizes new/modified files). Also remember `.` means the current directory.

Before we upload all the files, let's check what `git` will be uploading (all the files that `git` will upload should now appear in green):

{% filename %}command-line{% endfilename %}
```
$ git status
```

We're almost there, now it's time to tell it to save this change in its history. We're going to give it a "commit message" where we describe what we've changed. You can type anything you'd like at this stage, but it's helpful to type something descriptive so that you can remember what you've done in the future.

{% filename %}command-line{% endfilename %}
```
$ git commit -m "Changed the HTML for the site."
```

> __Note__ Make sure you use double quotes around the commit message.

Once we've done that, we upload (push) our changes up to GitHub:

{% filename %}command-line{% endfilename %}
```
$ git push
```

### Pull your new code down to PythonAnywhere, and reload your web app

* Open up the [PythonAnywhere consoles page](https://www.pythonanywhere.com/consoles/) and go to your **Bash console** (or start a new one). Then, run:

{% filename %}command-line{% endfilename %}
```
$ cd ~/my-first-blog
$ git pull
[...]
```

And watch your code get downloaded. If you want to check that it's arrived, you can hop over to the **Files tab** and view your code on PythonAnywhere.


* Finally, hop on over to the [Web tab](https://www.pythonanywhere.com/web_app_setup/) and hit **Reload** on your web app.

Your update should be live! Go ahead and refresh your website in the browser. Changes should be visible. :)

