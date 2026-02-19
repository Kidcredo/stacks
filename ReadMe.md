# Stacks

A curated collection of Docker Compose stacks for self-hosting various services. This repository provides easy-to-deploy configurations for development, monitoring, productivity, and more.

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

## Network Setup
Many stacks in this repository rely on an external Docker network named `kidcredo`. Create it with the following command:

```bash
docker network create kidcredo
```

## Usage

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yourusername/stacks.git
    cd stacks
    ```

2.  **Navigate to a stack directory:**
    ```bash
    cd <stack-name>
    ```

3.  **Configure Environment:**
    Copy the example environment file and adjust variables as needed.
    ```bash
    cp .env.example .env
    nano .env
    ```

4.  **Deploy the Stack:**
    ```bash
    docker compose up -d
    ```

## Available Stacks

### Development & Tools
-   **[ChartDB](chartdb/)**: Database design editor for visualizing and designing database schemas.
-   **[Code](code/)**: Deploy [VS Code Server](https://github.com/coder/code-server) (code-server) in a browser.
-   **[Git](git/)**: Self-hosted git service (Gitea/Forgejo).
-   **[Termix](termix/)**: Terminal in the browser.

### Monitoring & Administration
-   **[Monitoring](monitoring/)**: Monitoring stack featuring [Uptime Kuma](https://uptime.kuma.pet/) for tracking service uptime.
-   **[Networking](networking/)**: Network utilities and management tools.
-   **[Vaultwarden](vaultwarden/)**: Unofficial Bitwarden compatible server written in Rust.

### Productivity & Office
-   **[Mail](mail/)**: Mail server or client configuration.
-   **[Sheets](sheets/)**: Spreadsheet application.
-   **[Documentation](documentation/)**: Documentation platform (e.g., BookStack, Outline).

### Media & Creative
-   **[Media](media/)**: Media server stack (e.g., Jellyfin, Plex).
-   **[Photos](photos/)**: Photo management solution (e.g., Immich, PhotoPrism).
-   **[Data Visualization](data-visualization/)**: Tools for visualizing data (e.g., Metabase, Grafana).
-   **[Design](design/)**: Design tools (e.g., Penpot).

### Miscellaneous
-   **[Langflow](langflow/)**: UI for LangChain.
-   **[Link](link/)**: Link management.
-   **[Start](start/)**: Dashboard or start page (e.g., Homepage, Dashy).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
