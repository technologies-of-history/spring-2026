---
layout: page
draft: false
title: Digital Tools 1
---
# Communicating Simply with Markdown, Hugo, and GitHub
By now you've created a [GitHub](https://github.com) account, practiced opening a repository, making changes to a file, making a pull request, and merging branches with GitHub's [Hello World](https://guides.github.com/activities/hello-world/) tutorial. You've followed the [Markdown lesson](https://programminghistorian.org/en/lessons/getting-started-with-markdown) on the Programming Historian, so you know how to style your text files with Markdown syntax. We've practiced authoring Markdown files in class, but now it's time to do it on your own and create content for our course blog. You'll be following these same steps to create and submit the rest of your Digital Tools assignments, so it's very important for you to get the hang of these basic steps now.

## Step 1: Think about downloading a text editor

All of your digital assignments this semester will be authored in Markdown, which means 
you can't use Google Docs or Microsoft word to create them. As you know, you can always 
create Markdown files (.md) directly in GitHub, but if you'd like to be able to complete 
your assignments offline, save your work on your own machine, and preview your work in a 
local development environment on Hugo, then you will want to use a text editing program to 
write and save your .md files. If you've done some programming/coding 
before, you likely already have a favorite text editor, and you should keep using it. If not, 
I really like [Visual Studio Code](https://code.visualstudio.com/) which can run on MacOS, Windows, or Linux and
integrates directly with GitHUb. It's become the standard text editor in the field as it incorporates GitHub's AI help
for coding.

## Step 2: Take a look at an existing post

1. Open the class repository that you've forked into your personal GitHub account. 
2. Find the **content** folder and open it; then find the **posts** folder and open that. 
3. You'll see a single file in there titled **2024-11-04-Welcome to our course.md**. This is the Markdown file for the blog post that appears on the homepage of our course website. 
4. Note the file naming conventions. All of the blog posts created for our site must be named 
in the same way: **yyyy-mm-dd-your title.md**.
5. Click on the **2024-11-04-Welcome to our course.md** file in your GitHub repository, and then click on the pencil icon in the upper right to edit the file. You should now see the post written in Markdown with a header at the top 
that looks like this:

 ```
 ---
 layout: post
 bookTOC: false
 draft: false
 title: Welcome to our course!
 ---
 ```

6. Note the formatting of this file. The heading at the top is very important, and every post you write to submit a Digital Tools Assignment must contain these items:
- `layout: post` tells our Hugo builder to use the layout for a blog post for the Markdown that follows. Other pages in the `docs` folder are formatted as `page`, which tells Hugo to use a different layout for the Markdown that follows.
- `bookTOC: false` tells our Hugo builder not to include a right-hand menu with sections and sub-sections listed as a table of contents. If you did want that feature for a `post` or `page`, you would write `true` after the colon.
- `draft: false` tells Hugo to go ahead and serve this page to the website. If you were to write `true` after the colon, Hugo would recognize that this page is still in draft format, and not ready for publishing to the site.
- `title: Welcome to our course` is pretty self explanatory. You should type whatever title you'd like for your post after the colon.


## Step 3: Create a new post file in which to compose your assignment

(Note: the following instructions are for those of you brand new to GitHub, who don't use 
GitHub desktop or a text editor. This is the *most basic* 
way to add a file to your repository, but if you already know how to push changes and commit 
via those other platforms, go right ahead.)

__If you're working directly in GitHub:__
1. Return to the main course repository by clicking **spring-2026** at the top left of the page.
2. Create a new branch in our course repository by clicking the arrow to the right of **main** in the branch menu. In the text box that appears, type in the name of the new branch you'll create using the following naming convention: **lastname-dt1**.
3. Below that text box, click the option that appears that says **Create branch: lastname-dt1**.
4. Within in this new branch, click the **content** folder, and then the **posts** folder. 
5. At the top right, click **Add New File** and select **Create New File** to open GitHub's text editor.
6. Be sure to name the file according to the following naming conventions: **yyyy-mm-dd-your title.md**. ALL posts you create for this course blog must follow these exact naming conventions.

__If you're writing your posts in a text editor rather than on GitHub:__
1. Open your text editor of choice and create a new create a new Markdown file with the appropriate naming conventions: **yyyy-mm-dd-your title.md**. 

## Step 4: Write your post

Using appropriate Markdown syntax, Write a 2–3 paragraph post reflecting on the relationship between the
nature or format of a communication technology and the kind of knowledge that technology can
produce. Historians have suggested, for example, that alphabetic writing enabled 
the development of philosophical thought in Greece that was markedly different from that of ancient
Mesopotamia, with its cuneiform syllabary. In what ways do we see a similar relationship between
the principles of static computing and the production of digital scholarship? Are historians
arguments constrained or shaped by the digital tools available to them? How might the digital environment transform
historians' scholarship?

To receive full credit for this assignment, be sure to draw comparisons between the arguments expressed by Goody and Van De Mieroop
in their respective articles and those you develop related to digital communications. Use parenthetical citations (lastname page#)
 to cite these works if necessary.

## Step 5: Commit your post

1. After you create this Markdown file and fill it with your content, **Commit changes...** to save the file to your branch. Every time you do something in the file, you'll write up a brief description of what you changed and click, **Commit** to save. Be sure to select the option to commit to **your** new branch, **lastname-dt1**.
2. By keeping a record of these changes in these **Commits**, you're making it possible to revert back to a previous version of the file at any time.


## Step 6: Create a pull request

Once you're happy with your post and ready to submit the assignment, it's time to notify the developer (me) that you'd like the post to be merged into the **main** branch of the site so that it can be served to the website.

1. Click **spring-2026** to return to the main repository.
2. Be sure to check and make sure you're in your **lastname-dt1** branch.
3. In the menu at the top of the page, click **Pull requests**. 
2. Click the green button **New pull request**. 
3. You'll now see a gray box at the top that shows you the **base** repository you'll be sending your changes to and the **head** repository, which is yours. NOTE: Be sure that yours is the **head** and the main branch is the **base**.
4. Name your pull request **LastName_dt1** and then click **Create pull request**.

Ok, that's it! You've written a blog post in Markdown and followed the standard GitHub workflow to send it to our class site. Pat yourself on the back, and know that you'll do it all over again for the next four assignments.
