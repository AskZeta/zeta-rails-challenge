# Zeta Rails Code Challenge

Hello! Below are the instructions for a code challenge we'd like you to prepare. Please limit yourself to a reasonable amount of time on your solution, we want to respect your time but ask for a small commitment to see your skills in action.

## The Challenge

Write a simple app that queries and displays Github issues from the (rails)[https://github.com/rails/rails] repository.

#### Product Requirements

- As a user, I can go to the app and view a list of issues for the Rails project
- As a user, I can filter the issues by their state (open, closed, all)
- As a user, I can click an issue to see more details about it (should include title, url, description, labels, author)
- Include at least one item from the #extraFeatures section

#### Design Requirements

- It should look and feel easy to use and simple, but pleasing
- It should have some degree of styling applied to the elements

#### Technical Requirements

- Be launch-able from the command line and browsable in the browser
- Built in Rails
- If using a database, use PG
- Include a readme of how to install any necessary dependencies and launch the app

## Extra Features

Time permitting, choose one or several of the following features and implement them.

- Instead of just making json data available to your views, build non-database models for the issues ( e.g. @issues = issues_json.map{ | data| Issue.from_github_params(data) } )
- Build a data scraping service in the app (can be run by console if needed or a rails runner script) that queries issues and writes them to a model
- When viewing the issue, also display any comments it has received.
- Use Redis or an in-memory cache to cache responses

Your solution will be used as the basis of a code reviewing and pairing interview. Be prepared to talk about your code, why you made certain decisions, and be ready to walk another developer through your codebase.

## How to Submit

Create a private repo in github and add @khopkins218 as a collaborator

## Helpful tips:

- https://api.github.com/repos/rails/rails/issues
- https://developer.github.com/v3/issues/#list-repository-issues
