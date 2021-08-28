# Case Study


## Introduction
**`include <TYPE>`** is a web app portal that'll help it's users to manage and 
track their projects in an efficient and structured manner. Easy to access, 
anyone who's part of a project can use this portal for their benefit, be it 
a school student or a professional. It helps them to keep track of their 
day-to-day tasks, their time management and the overall progress of their 
project in a seamless and efficient way. A user friendly application with an 
awesome UI/UX that assists devs and managers to plan and collaborate better 
resulting in a much efficient and effective hierarchy of management and team 
work.

---

## Tech Stack 

- ### Frontend 

    - #### React
        For the frontend we initialy wanted to go with 
        [Blazor](https://blazor.net), which is a frontend framework of .NET 
        written in C#, and the primary reason behind it was we were already 
        using C# in the backend, in the form of ASP.NET Core, so it was 
        obvious to choose Blazor because it would've made our lives lot easier 
        coding in only one language.

        We made a demo app using Blazor and it was great except just one 
        problem, **App Size**. A fresh Blazor app weighs about 1.6 MB, which 
        was quite noticeable through the delay that we were facing during the 
        first launch of the app. This was a kind of a deal-breaker for us 
        because we didn't want the first experience of our app to feel slow.

        Since Blazor was out, we were looking into some other popular choices. 
        We decided we'd go with React, which weighs arond 43 KB. Vue was also enticing but in the end 
        we went with React because of it's Component-Wise-Development nature 
        where each UI component can be written into small compnents and 
        they can be easily re-used elsewhere.

    - #### TypeScript
        This was honestly an easy decision! TypeScript makes our lives a lot 
        easier. There are countless advantages of using TS, better 
        intellisense, better debugging, and most importantly, TS is **typed**, which makes it a lot easier to detect bugs in development.
    
    - #### Bootstrap 

    - #### GitHub Pages [for Hosting]

- ### Backend 

    - #### ASP.NET Core [with C#]
        This was again an easy decision to make. There were 2 reasons why we 
        went with ASP.NET Core. One, it's **FAST**, infact, ASP.NET Core is 
        **THE FASTEST** Backend framework out there. And two, one of our devs 
        was nicely experienced with C# programming.

    - #### PostgreSQL
        For the Database, we honestly could've used either Microsoft SQL 
        Server or MySQL or PostgreSQL. The ONLY reason we went with the last 
        option was because PostgreSQL was the only one which was natively 
        supported by Heroku (the Cloud that we're using).
    
    - #### Docker
        We're using Docker Containers to deploy our Backend App to the Cloud 
        in a containerized and isolated manner. Again, this makes the dev's 
        lives a lot easier. Mainly because almost all the popular Cloud 
        providers like Azure, AWS, GCP and Heroku have dedicated support for 
        docker conatiners. So even if Heroku doesn't natively support .NET, 
        we can use a .NET based Docker Container to deploy to Heroku. Sweet!

    - #### Heroku [for Hosting]
        Why not Azure or AWS or GCP? 
        <br>
        Because Heroku is FREE and doesn't require a Credit Card to Sign Up.

---

## Currently Implemented Modules

- ### Sign Up

- ### Log In / Out

---

