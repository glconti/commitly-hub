# commitly

`commitly` is a Git CLI extension that generates commit messages using an AI service.

## Installation

To install the CLI tool, download the latest release from the [GitHub releases page](https://github.com/glconti/commitly-hub/releases).

## Usage

To use the `commitly` command, simply run:

```sh
commitly
```

To preview the commit messages before committing, use the `--preview` option:

```sh
commitly --preview
```

## Configuration

To configure the `.gitconfig` file with the API key, add the following section to your `.gitconfig` file:

```ini
[commitly]
    apiKey = YOUR_API_KEY_HERE
```

Replace `YOUR_API_KEY_HERE` with your actual API key.

To set the `commitly.api-key` using the command `git config --global`, run the following command:

```sh
git config --global commitly.api-key YOUR_API_KEY_HERE
```

Replace `YOUR_API_KEY_HERE` with your actual API key.

## Examples

Here are some examples of how to use the `commitly` command:

```sh
# Generate a commit using the AI service
commitly
```

```sh
# Preview a commit using the AI service, then commit it
commitly --preview
```

```sh
# Generate maximum 2 commits using the AI service
commitly --max 2
```

## Config Command

To read the current configuration, use the `config` command:

```sh
commitly config read
```

## Update Command

To update the CLI tool, use the `update` command:

```sh
commitly update
```

The command will output a generated commit message based on the changes in your repository.
