# phpswitch

A simple Bash script to easily switch between different PHP versions on macOS using Homebrew. 

## Features

- Automatically install the specified PHP version if it’s not already installed.
- Unlink the current PHP version and link the specified version.
- Update your shell configuration to use the specified PHP version.
- Reload the Zsh shell to apply the changes.

## Requirements

- macOS
- [Homebrew](https://brew.sh/)
- Zsh shell

## Installation

1. **Download the `phpswitch` script:**

    ```bash
    curl -O https://raw.githubusercontent.com/yourusername/phpswitch/main/phpswitch
    ```

2. **Make the script executable:**

    ```bash
    chmod +x phpswitch
    ```

3. **Move the script to a directory in your PATH, e.g., `/usr/local/bin`:**

    ```bash
    sudo mv phpswitch /usr/local/bin/
    ```

## Usage

Use the script by specifying the desired PHP version. For example, to switch to PHP 8.2:

```bash
phpswitch 8.2
```

## Troubleshooting

**PHP Version Not Changing**

If the PHP version does not change after running the script, try the following:

Ensure Homebrew is installed and up to date:

```bash
brew update
```

**Verify that the PHP version is installed:**

```bash
brew ls --versions php@<version>
```

**Manually source your .zshrc file:**

```bash
source ~/.zshrc
```

**Open a new terminal session and check the PHP version:**

```bash 
php -v
```

## Common Errors

- **Homebrew not found**: Ensure Homebrew is installed and added to your PATH.

- **Permission denied**: Ensure you have the necessary permissions to move the script to /usr/local/bin or choose a different directory in your PATH.
- 
## Contributing
Feel free to fork this repository, submit issues and pull requests, or suggest new features.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
