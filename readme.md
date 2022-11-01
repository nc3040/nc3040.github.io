---
layout: default
---

# Host Your Resume

Follow this readme if you want to host your resume publicly on a staticly generated website for free using GitHub Pages!

[Demo website](https://nc3040.github.io)

![Resume after it's hosted](https://cdn.discordapp.com/attachments/484229849955827712/1037111899168444506/chrome_2022-11-01_16-09-13.gif)

## Uploading Your Own Resume

### Pre-requisites

You'll need a couple things before you can follow this guide:
- A resume using Markdown
    - See [more resources](#more-resources) if you need a guide to learn Markdown.
- A GitHub Account
    - If you don't already have one, head over to [github.com](https://github.com) to create a new account.
    - When prompted, choose to stick with the free plan for Github as we won't be needing any premium features.
- The git commandline tools
    - To upload our resume to GitHub, we need the Git command line tools installed. 
    - Follow [GitHub's guide to install git](https://github.com/git-guides/install-git) for the operating system you are using.
- The Visual Studio Code text editor
    - We'll be using Visual Studio Code to write and preview our resume. 
    - Download the editor for your operating system on the [Visual Studio Code website](https://code.visualstudio.com/).
    - You can leave all of the options in the installer at their defaults.

### Setting Up The GitHub Repository

1. Navigate to [GitHub](https://github.com/) and login to your account.
2. Next navigate to [this repository](https://github.com/nc3040/nc3040.github.io)
    - This repository contains a resume template that we'll use for formatting our own.
3. Click the `Fork` button in the top right of the page.
4. Fill out the information for this forked repository as follows:
    - For `Repository name`, enter your GitHub username followed by `.github.io`. For example, `nc3040.github.io`.
    - Leave the other options at their defaults.
    - Choose `Create fork`.
5. Click the `Settings` tab at the top of the page, then select `Pages` in the left sidebar.
6. Ensure `Deploy from a branch` is chosen in the dropdown for `Source`, then choose `gh-pages` in the `Branch` dropdown.
7. Press `Save`.

That's it! We now have a copy of the resume template that we can edit.

### Editing Our Resume in Visual Studio Code

1. Open Visual Studio Code (VS Code).
2. On the start screen, choose `Clone Git Repository...`.
3. Choose `Clone from GitHub` in the window that appears at the top of the screen.
4. When prompted to sign in to GitHub, choose allow then follow the login process in your browser.
5. After logging in, choose the repository we just forked from the list.
6. Create a folder somewhere on your PC to download the repository to.
7. Choose to `Open` the cloned repository when prompted.
8. In the file explorer on the left side, open the `_config.yml` file.
9. Add your name to the `title` property on line 1.
10. Replace the `url` value on line 2 with your username followed by `github.io` like you named the repository, for example, `nc3040.github.io`.
11. Save the file.
12. In the file explorer again, open `index.md`.
13. Enter all of your resume content written in Markdown. 
    - Make sure to keep the metadata on the first 4 lines of this file untouched.
14. Preview your formatting by right clicking the tab for this `index.md` file at the top of VS Code and choose `Open Preview`.

### Uploading our Resume to GitHub

1. In the bottom section of VS Code, click the Terminal tab
2. Type the following commands, making sure to replace the email and name in the commands:

```
git config --global user.email "example@email.com"
git config --global user.name "Your Name"
```

3. In the far left column in VS Code, click the tab named `Source Control`
4. Enter a message for the commit, such as `Add my resume`
5. Press `Commit` and confirm to stage all files when prompted.
6. Sign in to GitHub using your browser when prompted.
7. Press the big `Sync` button.

### Done!

Your resume is now being deployed on GitHub Pages! This can take up to an hour the first time. When it's complete, you can find it at `https://[username].github.io` where `[username]` is your GitHub username.

## More Resources

- Check out [Markdown Tutorial](https://www.markdowntutorial.com/) if you need to learn Markdown syntax.
- Check out Andrew Etter's book [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) to learn more about communicating technical content effectively.
- Check out [Jekyll Themes](https://jekyllthemes.io/) if you are interested in spicing up the look of your resume even more.

## Authors and Acknowledgements

- ankitsultana for their [Researcher Jekyll template](https://github.com/ankitsultana/researcher).
- Kunal Rajpal, Alborz Khakbazan, and Tristan Dyck for peer reviewing this readme and resume.

## Frequently Asked Questions

### Why is Markdown better than a word processor?
Markdown allows us to quickly write content with basic formatting syntax, then convert that basic syntax into any document format we want. In this guide we turn our Markdown into a static HTML website, but Markdown can also be converted into other formats like PDF. That means we can write out content quickly in one place and then easily have it formatted best for any medium that we want to share it by!

### How do I update my resume content after uploading it the first time?
You can edit the `index.md` file with any new changes, then just follow steps 3-7 under `Uploading our Resume to GitHub` again to commit and push your new changes.

