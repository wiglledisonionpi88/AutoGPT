# Installing Dependencies on macOS and Linux

This page summarizes the packages you need before running AutoGPT on macOS or Linux. It references the full setup guides for the Platform and Classic versions.

## AutoGPT Platform

Follow the [self-hosting guide](../platform/getting-started.md) for detailed steps. Ensure these tools are installed:

- **Node.js** – required for the frontend
- **Docker** (with Docker Compose)
- **Git**

Verify the installations:

```bash
node -v
npm -v
docker -v
docker compose -v
git --version
```

## AutoGPT Classic

See the [classic setup guide](../classic/setup/index.md) for full instructions. On macOS and Linux you need:

- **Python 3.10+**
- **Poetry**

Verify Python and Poetry:

```bash
python3 --version
poetry --version
```

## Providing Environment Variables

Both the Platform and Classic setups rely on an `.env` file for API keys and other options.

1. Copy the example file:
   - Platform backend: `cp autogpt_platform/.env.example autogpt_platform/.env`
   - Platform frontend: `cp autogpt_platform/frontend/.env.example autogpt_platform/frontend/.env`
   - Classic: `cp classic/original_autogpt/.env.template classic/original_autogpt/.env`
2. Edit the new `.env` file and add the variables required for your services.

Refer to the [configuration reference](../classic/configuration/options.md) for available variables.
