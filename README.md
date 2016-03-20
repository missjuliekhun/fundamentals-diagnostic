![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Fundamentals Diagnostic

A consultant will lead you through retrieving and responding to the diagnostic.

For the diagnostic itself, you have 30 minutes.

## Instructions

### Retrieve diagnostic from Github

#### Open the repository on github.com

If necessary, login to GitHub.  If you are not logged in, the `Sign in` button will be at the top right of the page when you navigate to https://github.com.

Navigate to this repository in Chrome.  The URL should be in slack forum.

#### Fork the repository

Click the Fork button in the upper right hand corner of the page.

![Github Fork](https://help.github.com/assets/images/help/repository/fork_button.jpg)

GitHub creates a copy of the repository and redirects the browser.

#### Create a folder to hold diagnostics

Open a terminal window then at the shell prompt:

```sh
cd ~
mkdir wdi
cd wdi
mkdir diagnostics
cd diagnostics
```

The first `cd ~` - change directory - ensures that you start in your home directory/folder.

`mkdir` creates a new directory/folder with the supplied name.  If you get an error message that includes `File exists` when you run `mkdir` it probably means you've already created the directory and can move on to the following `cd`.

#### Clone the repository

On GitHub, in your copy of the repository, find the clone URL widget - SSH/HTTPS drop-down, corresponding URL text-box, and `Copy to clipboard` button (centered in the following image).

![Remotes](https://help.github.com/assets/images/help/repository/remotes-url.png)

Before copying the clone URL to the clipboard, use the drop-down to select `SSH`. In [Which remote URL should I use?](https://help.github.com/articles/which-remote-url-should-i-use/) GitHub recommends using `https` remotes.  We will always use `ssh` remotes during your training.

Click the 'Copy to clipboard' button.

![Copy clone URL to clipboard](https://help.github.com/assets/images/help/repository/clone-repo-clone-url-button.png)

**Remember** it should say `SSH` in the drop-down when you do.

Back in the terminal (you should still be in the `diagnostics` directory created above):

```sh
git clone
```

Then paste the copied clone URL, run the command, and change into the newly created directory:

```sh
git clone git@github.com:<GitHub username>/fundamentals-diagnostic.git
Cloning into 'fundamentals-diagnostic'...
remote: Counting objects: 5, done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 5 (delta 0), reused 4 (delta 0), pack-reused 0
Receiving objects: 100% (5/5), done.
Checking connectivity... done.
cd fundamentals-diagnostic
```

### Complete Diagnostic

Create a `response` branch then open `diagnostic.md` with atom.

```sh
git branch response
git checkout response
Switched to branch 'response'
atom diagnostic.md
```

You may use any resource, other than someone else in the workspace, to help you complete the diagnostic.

Rendered markdown may be viewed by following [this link](diagnostic.md).

You should delete `_Replace this text with your answer._` following each questions and replace it with your answer.  Code answers need not be in markdown.

### 3) Turn in Diagnostic


#### Stage changed files

```sh
git status
On branch response
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   diagnostic.md

no changes added to commit (use "git add" and/or "git commit -a")
git add diagnostic.md
```

#### Create a git commit

```sh
git status
On branch response
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   diagnostic.md

git commit
```

Atom will open a text file containing comment lines (starting with a `#`) describing the changes being committed.  These lines are not included in your commit message.

Enter `Fundamentals diagnostic response` as the headline.  Leave a blank line then enter

```sh
git commit

[response 29a63bc]
 1 file changed, 25 insertion(+), 6 deletion(-)
$
```

#### Push changes to GitHub

```sh
git push origin response
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 304 bytes | 0 bytes/s, done.
Total 3 (delta 2), reused 0 (delta 0)
To git@github.com:<GitHub username>/fundamentals-diagnostic.git
 * [new branch]      response -> response
$
```

#### Create a Pull Request

We'll follow the GitHub help article, [Creating a pull request](https://help.github.com/articles/creating-a-pull-request/) skipping step 4.

## Additional resources

Additional GitHub help articles.

- [Fork A Repo](https://help.github.com/articles/fork-a-repo/)
- [Cloning a repository](https://help.github.com/articles/cloning-a-repository/)

## [License](LICENSE)

Source code distributed under the MIT license. Text and other assets copyright
General Assembly, Inc., all rights reserved.
