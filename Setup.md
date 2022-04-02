# Repository Setup Instructions

The course's _upstream_ repository (located at `https://github.com/Tech-at-DU/ACS-3110-Trees-Sorting`) contains course materials including the schedule, class topics, challenges, starter code, unit tests, slides, and links to resources. It will be updated throughout the course, so you will need to regularly _pull_ from it to get new materials. (Note that you cannot _push_ to the course's upstream repository.) However, you can _clone_ this repo to get upstream changes and also push your code to your own repo.

**Important:** Please follow these instructions _exactly_ to correctly set up your clone of this repository. If you skip a step or do them out of order, it may not work.

## Step 1: Set Up Your Local Course Repo Clone

1. **Clone** (do not _fork_) this repo from GitHub onto your local computer.

  - First open your terminal and navigate into the folder where you keep your course material and projects: `cd ~/Development/Courses` (or something similar for your folders)

  - Then run this command to _clone_ the course repo: `git clone https://github.com/Tech-at-DU/ACS-3110-Trees-Sorting.git`

  - Now navigate into the new folder Git just created: `cd ACS-3110-Trees-Sorting`

2. [**Create a new empty repo** on GitHub](https://github.com/new) also named `ACS-3110-Trees-Sorting` and **do not** initialize it with a ReadMe. (Creating a _new_ repo instead of a _fork_ allows you to earn credit towards your GitHub commit streak.)

3. **Set the `origin` remote's URL** on your local repo to point to your new repo on GitHub: `git remote set-url origin https://github.com/<your-username>/ACS-3110-Trees-Sorting.git`

4. **Push your local repo** to your _remote_ GitHub repo to link your `master` branch to your `origin` remote: `git push -u origin master`

5. **Commit your code** to your local repo frequently (each time you've made meaningful progress).

6. **Push your commits** to your remote GitHub repo when you want to publish and backup your code: `git push` (the `-u` in the previous command lets you omit `origin master` afterward).

## **Step 2:** Connect Local Clone To _Upstream_ Repo On Github

1. Add this course's upstream repo as another _remote_ to your local repo with: `git remote add upstream https://github.com/Tech-at-DU/ACS-3110-Trees-Sorting.git`

2. Verify that you have two remotes: `origin` (with your username in the URL) and `upstream` (with `tech-at-du`): `git remote -v`

3. When you want to access new course materials, first be sure you've committed and pushed your recent work (run `git status` to check) and then _pull_ from the course's upstream repo with: `git pull upstream master`

> **Note:** To avoid unnecessary merge conflicts when pulling changes from `upstream`, write all of your project code inside the `Code` folder and **do not** modify or delete any existing files outside of the `Code` folder that may change upstream.
