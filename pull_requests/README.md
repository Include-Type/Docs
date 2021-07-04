# Instructions focusing on Pull Requests

## How to make a Pull Request using Branches
- First create a Local Branch
    ```shell
    $ git checkout -b <your_name>
    ```
- Then work within your `<your_name>` branch.
- After you've finished coding and you're ready to commit, pull the code from the `main` branch once.
    ```shell
    $ git pull origin main
    ```
- Check if there are any clashes or not. If there are any, fix them. If there are clashes, VSCode will give you some options. Always use the **Accept Incoming Changes** option!
- After fixing all the clashes, **Add, Commit and Push** to `<your_name>` branch.
    ```
    $ git add <files>
    $ git commit -m "A nice commit message detailing the features/fixes"
    $ git push origin <your_name>
    ```
- After pushing your code to your branch, head over to your branch in GitHub and you'll see a big **Pull Request** button. Use that to initiate a Pull Request.
- After your pull request is merged by any org. member and you can see your code reflected in the remote's `main` branch, delete both of your **Remote** and **Local** branches (the one having the name `<your_name>`).
    - To remove the **Remote** branch, use GitHub's **Branches** menu.
    - To remove the **Local** branch, use:
        ```shell
        $ git checkout main
        $ git branch -D <your_name>
        ```
- Now that you'll be in the `main` local branch, pull the code from the remote's `main` branch to do a final sync.
    ```shell
    $ git pull origin main
    ```
And that's it! 🎉  
Follow the above steps for your next Pull Request.