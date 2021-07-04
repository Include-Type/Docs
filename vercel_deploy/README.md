# Instructions focusing on how to deploy the app to Vercel for testing and production purposes.

## Deploy to Vercel using a Fork
Since Vercel doesn't allow deployments from Private Org. Repos in the Free Tier, hence we need to make a **Fork** of the Private Org. Repo.  
In order to fork a repo, use the **Fork** button at the top-right corner. That'll fork that particular repo into your personal GitHub account.    

- First go to [Vercel's home page](https://vercel.com/) and create an account for Free.
- Then connect your GitHub account.
- After that select that Forked Repo and click on **Import**.
- Vercel will ask for the **Name** of the app and few other details like the **Framework** and **Build Commands**. Since they already have a pre-built template made for React, we don't have to mess with those settings, Vercel will do that for us.
- After that, Vercel will automatically create a CI/CD Pipeline for our app. Now everytime we **Push** to our **Forked Repo**, our app will be automatically deployed using that pipeline.

## Git Workflow for deploying to Vercel using a Fork
- First copy the Git Link of the **Forked** repo.
- Then go to the **main local repo** (from where the fork was made).
- Run:
    ```shell
    $ git remote -v
    ```
    The above command will show you the remote links of the main repo (from where the fork was made). Notice, those remotes will have an alias of `origin`.
- Now add the remote links of the forked repo:
    ```shell
    $ git remote add fork <Git link of the Forked Repo>
    ```
    Then verify once again:
    ```shell
    $ git remote -v
    ```
    You should see the remote links of the forked repo been added with the alias `fork`.
- That's it, then if you feel like to deploy the app, maybe for testing or for production, push your code to your **forked repo**:
    ```shell
    $ git push fork main
    ```
    After you push your code to the **forked repo**, your app will be automatically deployed using Vercel's CI/CD Pipeline.