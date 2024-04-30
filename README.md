# First Contributions using Git and GitHub

This is a guide for beginners on how to make a contribution using Git and GitHub. 
If you are looking to make your first contribution, follow the steps below.

As a complement to the instructions below, feel free to watch [this video](https://youtu.be/1UhCR-xHZOM) where I do all the following steps in real time. It takes about 15 minutes.

# 1. Create an account on GitHub. 
It is for free and should just take some minutes.

# 2. Install Git. 
[Here](https://docs.github.com/en/get-started/quickstart/set-up-git) is a tutorial on how to set up Git.

# 3. Fork this repository.
Click on the fork button on the top of this page. This will create a copy of this repository in your account.
<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/fork.png" alt="fork this repository" />

# 4. Clone the forked repository.
Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon. 
<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone this repository" />
<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/copy-to-clipboard.png" alt="copy URL to clipboard" />

Then, open a terminal and run the following git command:
```
git clone "url you just copied"
```
where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.


For example:

```
git clone https://github.com/this-is-you/make_a_pull_request.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.

# 5. Create a branch.

Change to the repository directory on your computer (if you are not already there):

```
cd make_a_pull_request
```

Now create a branch using the `git switch` command:

```
git switch -c your-new-branch-name
```

For example:

```
git switch -c add-Stephan-Huber
```
# 6. Make changes.

Now open the`I_am_a_data_scientist.md` file in a text editor. (You find this file in the repository.)
Add your name, your GitHub account and the paper that you want to reproduce to it. 
Don't add it at the beginning or end of the file. Put it anywhere in between. Now, save the file.

If you go to the project directory and execute the command `git status`, you'll see there are changes.

# 7. Add changes (staging).
Add those changes to the branch you just created using the `git add` command:

```
git add .
```

# 8. Commit changes.
Now commit those changes using the `git commit` command:

```
git commit -m "Add your-name to the list"
```

replacing `your-name` with your name.


# 9. Use Git Bash.
Open Git Bash and set your email and your nickname on GitHub:

```
git config --global user.name "FIRST_NAME LAST_NAME"
git config --global user.email "MY_NAME@example.com"
```

# 10. Push changes to GitHub.

Push your changes using the command `git push`:

```
git push -u origin your-new-branch-name
```

replacing `your-new-branch-name` with the name of the branch you created earlier.

*If you get any errors while pushing that refers to authentication failed something, go to [GitHub's tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) on generating and configuring an SSH key to your account. Alternatively, you can watch this [YouTube tutorial](https://youtu.be/m5SChqEi314)*

# 11. Submit your changes for review on GitHub.

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/compare-and-pull.png" alt="create a pull request" />

Now submit the pull request.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/submit-pull-request.png" alt="submit pull request" />

Soon I'll be merging all your changes into the main branch of this project. You will get a notification email once the changes have been merged.

## Where to go from here?

Congrats! You just completed the standard _fork -> clone -> edit -> pull request_ workflow that you'll often encounter as a contributor!

If you write a project report for the Hochschule Fresenius, don't forget to mention that you have successfully gone through that tutorial!



