# Open Cultivar

Open Cultivar is a community-driven database for plant cultivars and varieties. This project is built as a high-performance Jamstack website running at [opencultivar.com](https://opencultivar.com).

## Tech Stack

This project utilizes the following technologies:

-   **Static Site Generator:** [Hugo](https://gohugo.io/) - A fast and flexible static site generator written in Go.
-   **Headless CMS:** [Decap CMS](https://decapcms.org/) (formerly Netlify CMS) - A git-based headless content management system that allows for easy content updates.
-   **Authentication:** [Netlify Identity](https://www.netlify.com/products/identity/) - A service for handling user authentication, used here to allow users to log in and contribute.
-   **Git Backend:** [Git Gateway](https://www.netlify.com/docs/git-gateway/) - A Netlify service that allows Decap CMS to interact with the GitHub repository without requiring users to have a GitHub account.

## How it Works

Content is managed through the Decap CMS interface, which is accessible at `/admin`. When a user submits new content (like a new cultivar or a log entry), Decap CMS creates a new file in the git repository. The `editorial_workflow` mode is enabled, which means that submissions from non-technical users will be created as pull requests in the GitHub repository, awaiting approval before being published to the live site.

## Contributing

Contributions to Open Cultivar are welcome! Here's how you can help:

1.  **Fork the repository** on GitHub.
2.  **Clone your fork** locally.
3.  **Create a new branch** for your changes (e.g. a new species, cultivar, log entry or code change).
4.  **Make your changes** and commit them.
5.  **Push your changes** to your fork.
6.  **Submit a Pull Request** to the main repository.

Please ensure your code follows the existing style and conventions. If you find a bug or have a feature request, please open an issue.
