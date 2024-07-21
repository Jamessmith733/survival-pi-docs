---
sidebar_position: 1
sidebar_label: Tutorial
---

import TOCInline from '@theme/TOCInline';
import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

# How to contribute

This website is a community project for the community and by the community. It is fully open-source with the code being available at [GitHub](pathname://https://github.com/aleabodo/survival-pi-docs). It means that every member of the community can literally edit *anything* of the website and contribute to adding new information and posts to it.

## Some terms

These are some of the most important terms you should know when working with Git. I will be using them, so I recommend to at least skim over them.

<Tabs>
  <TabItem value="git" label="Git" default>
    Git is a powerful version control system that helps track changes to files and coordinate work on those files among multiple people. 
  </TabItem>
  <TabItem value="repo" label="Repository (Repo) 💾">
    A repository is a storage space where this project lives. It contains all the files and the history of all changes ever made to them. Repositories can be local (on your computer) or remote (on a server like [GitHub](pathname://https://github.com/aleabodo/survival-pi-docs)).
  </TabItem>
  <TabItem value="commit" label="Commit ✅">
    A commit is like a snapshot of your project at a specific point in time. Each commit contains information about what changes were made, who made them, and when. Think of it as saving your changes to a log book.
  </TabItem>
  <TabItem value="fork" label="Fork 🍴">
    A fork is a personal copy of someone else's repository that lives on *your* account. It allows you to freely experiment with changes and make commits without affecting the original project. Forking is often used when you want to contribute to a repository you don’t own (as we will see later).
  </TabItem>
  <TabItem value="pullrequest" label="Pull Request (PR) 📩">
    A pull request is a way to propose changes you've made (on your fork) to a project so that they can be reviewed and potentially merged ("*pulled*") into the original repository. As you will see later, you'll need to make a PR so I can review your commits before accepting them into the website.
  </TabItem>
</Tabs>

## Follow these 5 steps to make your first edit

1. **Create a GitHub Account** \
    [Create an account on GitHub](pathname://https://github.com/signup). Sign in with your new account.

2. **Click on *Edit this page*** \
    Visit any page you want to edit and scroll to the bottom. Click on the button `Edit this page`, redirecting you to the corresponding file on the [GitHub repository](pathname://https://github.com/aleabodo/survival-pi-docs). \
    ![Edit this page button](/img/wiki/edit-this-page.png)

3. **Follow the instructions to fork the Repo** \
    Since you don't own this repository, GitHub will ask you to create a Fork. Follow the instructions. \
    ![Fork this repository](/img/wiki/fork-this-repository.png)

4. **Edit the Page** \
    Now you can edit the website's code. Most pages, including the Wiki and Season pages, use Markdown, a simple format you might know from note-taking apps. To learn more, check out [this markdown cheatsheet](pathname://https://www.markdownguide.org/cheat-sheet/). To get started quickly, I recommend getting familiar with the existing text and checking out the [example page of a base](./example-page.md) and the corresponding code. 

    :::note[Some footnotes on editing:]
    - You can format pages however you see fit, not limited to specific templates.
    - All pages of the seasons and the Wiki are in the `/docs/` directory. The sidebar of the website will follow that directory tree.
    - Adding images is a little bit more involved since the GitHub website doesn't allow you to easily upload images. So if you want to add images to your page, just add the template image as below and send BuildingBrute your real images. He will handle the rest.
        ```markdown
        ![Pic](/img/placeholder.jpg)
        ```
    - When you create new files (on the sidebar is a *+* button), make sure you don't include any whitespaces in the file name. Also, it needs to have the file ending `.md` standing for *markdown*. Please make sure you familiarize yourself with the directory structure to keep it organized.
    :::

5. **Commit Your Changes** \
    Click on `Commit changes...` to create a snapshot of your edits on your forked repository. Please make a meaningful commit messages. Avoid messages like "LOL" or "Changed something". Describe your changes briefly and clearly; this helps the reviewer understand your edits.
    
6. **Create a Pull Request** \
  Review your changes and click `Create pull request` to propose merging your commits into the main repository. \
  ![Pullrequest](/img/wiki/pullrequest.png)

--- 

  :::tip
  You can make multiple commits on your account's forked repository before making a pull request. This is especially useful if you need to add multiple files like pictures for a page.
  :::

  :::warning[Keep your repo in sync before making subsequent Pull Requests!]
  Before making subsequent edits to your forked repository, you need to make sure that it's synced and up-to-date with the main repository, else you're editing old files. You can do that by clicking `Sync fork` on you repository's main page. You can see whether your fork is commits behind the main repository. You can also make PR from here. 

  ![Pullrequest](/img/wiki/sync.png)

  You can find your repository in your GitHub profile under `Your repositories`.
  :::