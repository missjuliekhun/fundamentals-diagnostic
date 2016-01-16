![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# Fundamentals Diagnostic

A consultant will lead you through retrieving and responding to the diagnostic.

For the diagnostic itself, you have 30 minutes.

## Instructions

### Retrieve diagnostic from Github

#### Open the repository on github.com

If necessary, login to GitHub.  If you are not logged in, the `Sign in` button will be at the top right of the page when you navigate to https://github.com.

Navigate to [this](#) repository in Chrome

#### Fork the repository


Click the Fork button in the upper right hand corner of the page.

![Github Fork](https://help.github.com/assets/images/help/repository/fork_button.jpg)

GitHub creates a copy of the repository and redirects the browser.

#### Create a folder to hold diagnostics

Open a terminal window then at the shell prompt:

```sh
$ cd
$ mkdir wdi
$ cd wdi
$ mkdir diagnostics
$ cd diagnostics
```

#### Clone the repository

On GitHub in Chrome, find the

From your bash terminal, clone your newly created Github repo by typing
  `git clone git@github.com:YOUR-USERNAME/wdi_1_ruby_diagnostic_prework.git`
  ![git clone](http://i.imgur.com/Vuk3ujAl.png)
Change into the `wdi_1_ruby_diagnostic_prework` by typing `cd wdi_1_ruby_diagnostic_prework`
Run `bundle install` to ensure you have all needed *ruby gems* on your system.

### 2) Complete Diagnostic

Using Sublime, edit the `diagnostic.md` file, and follow the instructions in the comments in the code.

You may run `ruby diagnostic.md` to make sure the syntax parses properly along the way. You may also run `rspec spec` to see which items you've currently got right, and which ones need improvement.

### 3) Turn in Diagnostic

Once completed:

#### Stage changed files

```sh
$ git add diagnostic.md
```

#### Create a git commit

```sh
$ git commit
```

#### Push changes to GitHub

```sh
$ git push origin response
```

#### Create a Pull Request

by going to `https://github.com/YOUR-USERNAME/wdi_1_ruby_diagnostic_prework/pulls` and hit the green "New Pull Request" button
![New Pull Request](http://i.imgur.com/RKGUz1sl.png)

- Hit the green "Create Pull Request" button now on the left side of the screen
![Create Pull Request](http://i.imgur.com/q8wczMZl.png)

- Now leave an additional comment and/or message, and hit the green "Create Pull Request" in the bottom right hand corner to finalize the PR.
  ![Finalize Pull Request](http://i.imgur.com/GZKSK8Xl.png)
