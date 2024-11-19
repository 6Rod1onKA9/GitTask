# Exploring GIT

**Objectives:**
- To master the basics of working with the version control system Git.
- Create and conﬁgure a project using the React and TypeScript template.
- Learn to use various tools for working with Git, including the command line and the graphical user interface of the IDE.

# Tasks:
**- Tutorial Review:**
Study the Git tutorial available at Git How To. Pay special attention to the ﬁrst 21 steps, which cover the basic operations with Git.

**- Choice of Development Tool:**
For this assignment, you may use one of the following Integrated Development Environments (IDE): WebStorm or Visual Studio Code. Ensure that the IDE is installed and conﬁgured to work with Git.

**- Using the Command Line:**
Use the command line to execute the Git operations described in the tutorial. This will help better understand the version control system process.

**- Using the IDE's Graphical Interface:**
Use the built-in features of the graphical interface of the chosen IDE to track changes in the repository. Demonstrate visually the results of the commands performed in the IDE for each step of the tutorial.

**- Visual Conﬁrmation of Changes:**
Provide screenshots or other visual conﬁrmations of the repository changes made for each of the ﬁrst 21 steps of the tutorial, using the graphical interface of the IDE.

**SOLUTION ->**
# Git Credentials

1) So firstly, we create a new project, where we can work with a file. For that, I chose such an IDE - **WebStorm**:

![image](https://github.com/user-attachments/assets/d6bd7d4f-c4cc-4141-98a4-432a2c7a659f)

2) Then we open the terminal run our very first commands. Let's have Git know my name and email:

![image](https://github.com/user-attachments/assets/d1937ca6-9483-4afb-abc7-46d459e53c30)

3) Then we will use `main` as the default branch name:

![image](https://github.com/user-attachments/assets/d3d47b31-de7f-4bdf-807d-2a2f1e22e248)

4) Now, we add the **Line endings treatment**, shall we?

![image](https://github.com/user-attachments/assets/2251ee70-c502-4c1d-9c48-d5f7b5f5304b)

# Creating a project

5) Now let's add an empty subdirectory named `work`, then create a `hello.html` file in it:

![image](https://github.com/user-attachments/assets/b340dd66-f1ff-42c6-aead-7c332d4c22e7)
![image](https://github.com/user-attachments/assets/52297eef-64ad-4293-a96f-a64c4bf13009)
![image](https://github.com/user-attachments/assets/97246acc-29c6-44f9-b0b0-94473d4daa77)

6) Then we run `git init` in order to create a Git repo from that directory:

![image](https://github.com/user-attachments/assets/9ea2d22b-a398-4c47-8124-bc0ace368813)

7) For now we can see, that the file has red colour. It is because, it has not been added yet. Therefore, let's add it:

![image](https://github.com/user-attachments/assets/1ebeb1ee-9edd-4f89-b41c-5127c0faf4a9)
![image](https://github.com/user-attachments/assets/c327a82c-afd9-4dcf-bf0f-97376744a5ae)
![image](https://github.com/user-attachments/assets/1e920e97-704b-41e9-8afd-631fc22cc082)

8) Now let's make our first commit. It is going to be a commit, that we added the `hello.html` file:

![image](https://github.com/user-attachments/assets/9dd9a571-4bbf-45ab-bd63-32d096142596)

# Checking the status of the repository

9) Now let's check the status of our repository. It says it has hidden file. Such files should not be committed because it is about configuration in your local environment. These file should be ignored:

![image](https://github.com/user-attachments/assets/9aeaf662-3ab0-43e8-bf55-e277edc4c5ce)

# Making changes

10) Let's add some `html` text in our file:

![image](https://github.com/user-attachments/assets/ec1942b1-b68d-4b56-a374-3cf5c89bcccf)

11) After that, we run the `git status` again, and see, what we got. Git knows `hello.html` file has been changed, but these changes are not yet committed to the repository:

![image](https://github.com/user-attachments/assets/33ae0949-ed42-4fc0-8494-ec6d13b9fe3a)

12) Let's make a commit of our changes and check the `git status` again:

![image](https://github.com/user-attachments/assets/e0d9d13f-2933-4811-8860-e50336015e9a)
![image](https://github.com/user-attachments/assets/13fa03aa-d696-4137-a8d6-0af0f618716b)

# History

13) Getting a list of changes made is a function of the `git log` command:

![image](https://github.com/user-attachments/assets/a328b38e-5a4a-4086-8e5b-44224f6d1882)

14) We can also see the one line history of commits:

![image](https://github.com/user-attachments/assets/ee0c0330-41b7-421b-bfda-cc04439abf13)

15) It is also possible to check the changes made within the last week for example:

![image](https://github.com/user-attachments/assets/95f9eddc-b535-4921-909e-b09b1bcae63b)

# Getting older versions

16) Lets get a hash of one of our previous commits again:

![image](https://github.com/user-attachments/assets/95f9eddc-b535-4921-909e-b09b1bcae63b)

17) Git make time traveling possible, at least for your project. The checkout command will update your working directory to any previous commit:

![image](https://github.com/user-attachments/assets/987aa5fd-9b85-40f5-90b1-885ad96bead4)

18) To return to the latest version of our code, we need to switch to the default `main` branch. We can use the `switch` command to switch between branches:

![image](https://github.com/user-attachments/assets/2931d3d2-474f-41a2-82fa-5fcd28d13497)

# Tagging versions

19) Let's create a tag for the 1st version. After that let's also see, what tags we are going to have as a result:

![image](https://github.com/user-attachments/assets/30c8abb7-603d-4511-b865-adac4b1ac8b9)
![image](https://github.com/user-attachments/assets/87a03de6-9ab9-4af9-9f6e-a90721ab6e1a)
(v0 was created as well, but manually in UI GIT)

# Cancel staged changes (before committing)

20) Let's get some changes in `hello.html` file:

![image](https://github.com/user-attachments/assets/ab525168-cfbf-495f-bbc9-b3b6c89378f9)

21) We stage the modified file:

![image](https://github.com/user-attachments/assets/4b968d9b-72ac-4395-a0ec-8151309ed8cd)

22) As usual, check the status:

![image](https://github.com/user-attachments/assets/83e04c42-95a2-4d18-a49f-7b764334f90f)

23) Then we reset the staging area to HEAD. This clears the staging area from the changes that we have just staged:

![image](https://github.com/user-attachments/assets/f942dce5-06ce-444a-af39-8faeea5c08da)

24) We can use the `checkout` command from the previous tutorial to remove unwanted changes from working directory:

![image](https://github.com/user-attachments/assets/a4925d78-f05b-4aed-a1c9-27e2024733f2)

# Cancelling commits

25) Not let's add some changes to file:

![image](https://github.com/user-attachments/assets/3010cc6a-f35e-4f93-a004-ee147e4206cf)

26) To cancel the commit, we need to create a commit that deletes the changes saved by unwanted commit:

![image](https://github.com/user-attachments/assets/d8810604-6517-4943-89b2-e2f1e7133dce)

27) Checking the log shows the unwanted cancellations and commits in our repository:

![image](https://github.com/user-attachments/assets/5638b011-778e-4da8-a6aa-c8e612f44df9)

# Removing a commit from a branch

28) Let us mark the last commit with `tag`, so you can find it after removing a commit:

![image](https://github.com/user-attachments/assets/d0d6f182-7d7e-4c63-9bf3-929453c92151)

29) Let us reset the branch to that point. As the branch has a tag, we can use the tag name in the `reset` command (if it does not have a tag, we can use the hash of the commit):

![image](https://github.com/user-attachments/assets/e0cbf00f-6b99-484a-ac0f-59fea0db14c3)

30) Let us take a look at ***all*** commits.

![image](https://github.com/user-attachments/assets/10598feb-d15e-481d-9b2b-63e6d088950d)

We can see that the wrong commits are not gone. They are not listed in the main branch anymore but still remain in the repository:

# Removing the `oops` tag

31) The `oops` tag has performed its function. Let us remove that tag and permit the garbage collector to delete referenced commit:

![image](https://github.com/user-attachments/assets/34c124af-89db-415d-b9a8-d4296b03e4f8)

# Amending commits

32) Let's put an author comment on the page:

![image](https://github.com/user-attachments/assets/aa442229-535a-4a78-93b7-7f47ae90ddf7)

33) Now let's save changes in the file and make a commit it:

![image](https://github.com/user-attachments/assets/94faec71-7a6d-4f79-aae8-b31f7f4bd8df)

34) After making the commit you understand that every good comment should include the author's email. Edit the `hello.html` page to provide an email:

![image](https://github.com/user-attachments/assets/bbfbea9f-28d7-4489-b76e-c019a2f2846f)

35) We do not want to create another commit for adding the email address. Let us change the previous commit and add an email address:

![image](https://github.com/user-attachments/assets/1012279b-29ca-4ed6-8776-74a4fa810f17)

36) Now view the history:

![image](https://github.com/user-attachments/assets/2feb2c84-75b2-4096-94d2-eb13fda715a4)

# Creating a branch

37) It is time to make our page more stylish with a touch of CSS. We'll develop this feature in a new branch called `style`.

![image](https://github.com/user-attachments/assets/1f5c2692-babb-43b3-92b4-50d9ee0bf649)

38) Now let's add the `style.css` file

![image](https://github.com/user-attachments/assets/431d1550-4fad-41b5-b2b0-6e1929629617)
![image](https://github.com/user-attachments/assets/07f50f6b-2bd9-4ed4-b89f-4fa5594e56ab)

39) Now we change `hello.html` to add `style.css`

![image](https://github.com/user-attachments/assets/a08f8e15-6437-4dd4-8253-bf23159779c5)
![image](https://github.com/user-attachments/assets/66bbf8c0-6daf-49e7-8cb5-47f8e7823bf5)

# Switching branches

40) To switch between branches, we use the `git switch` command.

![image](https://github.com/user-attachments/assets/3d1b1597-2dfe-4710-9d97-f44e102eb6fe)
![image](https://github.com/user-attachments/assets/c335ea50-ab92-4109-a5f3-28d958fc7baf)

Now we are on the `main` branch. As we can see, the `hello.html` has no traces `of style.css`. However, it is still in the repository, but we just can't see it from the `main` branch.

41) Let's return to the style branch

![image](https://github.com/user-attachments/assets/28a29751-53f6-4dfc-9463-2e4c97d5c022)

# Moving files

42) Git provides the capability to examine the change history of a specific file. Let's take a look at the change log for the `hello.html` file before we proceed with renaming it.

![image](https://github.com/user-attachments/assets/9da1bf08-afa6-476d-b9e0-c4a2489ae7d2)
![image](https://github.com/user-attachments/assets/8db59201-7eba-4bde-9dfb-19050ce420ed)

43) The `show` command is used to display the changes in a specific commit. Let's examine the changes in the `hello.html` file in the commit tagged with `v1`

![image](https://github.com/user-attachments/assets/52d63a49-1dc3-4cb5-810d-6a7ec54e79db)

44) Let's rename our `hello.html` file to `index.html` using the standard `mv` command and observe the outcome.

![image](https://github.com/user-attachments/assets/12ba7289-d31b-44c8-851b-1fe50a5a4fbf)
![image](https://github.com/user-attachments/assets/3b5d8f8a-c444-4246-9987-60eac5021c9a)

45) Let's move our `style.css` file to the `css` directory. We'll use the git `mv` command to ensure the move is recorded in Git's history as a move, not as a deletion and addition of a new file.

![image](https://github.com/user-attachments/assets/191abcec-da2c-4f48-a974-d7e7d54f1ccd)

46) Now we commit our changes and examine the change history of the `css/style.css` file. To see the file's history prior to its relocation, we'll need to include the `--follow` option.

![image](https://github.com/user-attachments/assets/b033c99d-20c9-409f-a245-3cee073787e7)

# Changes in the main branch

47) Let's create a file `README`.

![image](https://github.com/user-attachments/assets/4601a4d5-c831-4531-af89-a8ec1db9881d)
![image](https://github.com/user-attachments/assets/30a1c1ec-31fb-4315-944b-44a3dfec6a05)

# Viewing diverging branches

48) We now have two diverging branches in the repository. Let's use the following `log` command to view the branches and how they diverge.

![image](https://github.com/user-attachments/assets/222a54fd-868b-4cb0-89de-8b9719aadece)
![image](https://github.com/user-attachments/assets/4983aaee-9179-42ea-8106-42c39279cd6d)
![image](https://github.com/user-attachments/assets/9b6ccca8-5c2c-41f2-bf70-5dc695f50c21)

# Merging

49) Merging brings changes from two branches into one. Let us go back to the `style` branch and merge it with `main`.

![image](https://github.com/user-attachments/assets/18acda9d-2f39-4e74-875d-99cc73993115)
![image](https://github.com/user-attachments/assets/4243cdd7-ed2f-48b6-bf37-29c90ccbc7ad)
![image](https://github.com/user-attachments/assets/28a47afe-1aac-4075-999e-b5df0fb7bc37)
