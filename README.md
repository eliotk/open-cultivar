# Open Cultivar

Open Cultivar is a community-driven database for plant cultivars and varieties. This project is built as a high-performance Jamstack website.

## Tech Stack

This project utilizes the following technologies:

-   **Static Site Generator:** [Hugo](https://gohugo.io/) - A fast and flexible static site generator written in Go.
-   **Headless CMS:** [Decap CMS](https://decapcms.org/) (formerly Netlify CMS) - A git-based headless content management system that allows for easy content updates.
-   **Authentication:** [Netlify Identity](https://www.netlify.com/products/identity/) - A service for handling user authentication, used here to allow users to log in and contribute.
-   **Git Backend:** [Git Gateway](https://www.netlify.com/docs/git-gateway/) - A Netlify service that allows Decap CMS to interact with the GitHub repository without requiring users to have a GitHub account.

## How it Works

Content is managed through the Decap CMS interface, which is accessible at `/admin`. When a user submits new content (like a new cultivar or a log entry), Decap CMS creates a new file in the git repository. The `editorial_workflow` mode is enabled, which means that submissions from non-technical users will be created as pull requests in the GitHub repository, awaiting approval before being published to the live site.
