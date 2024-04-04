# Git Co-Author Utility

## Overview

This utility is designed to make it easier to add co-authors to your Git commits. It's a simple command-line tool that reads from a co-authors file and adds the appropriate co-author lines to your commit messages.

## Installation

To install the Git Co-Author Utility, clone the repository and add the project directory to the PATH.

## Usage

To use the Git Co-Author Utility, first create a co-authors file.

The utility expects this file to be present at `~/.gitauthors` or the path stored in the `COAUTHORS_PATH` environment variable.

This file should be an INI file, with each co-author represented as a separate section. Here's an example:

```text
[harry]
    name = Harry Potter
    email = hpotter@hogwarts.edu

[hermione]
    name = Hermione Granger
    email = hgranger@hogwarts.edu

[ron]
    name = Ron Weasley
    email = rweasley@hogwarts.edu
```

Then, when you're ready to commit, use the git coauthor command followed by the keys of the co-authors you want to add:

```bash
git coauthor -m "The commit message" -a harry -a hermione
```

This will add Harry and Hermione as co-authors to your commit.

For more information on the utility, consult the manual:

```bash
man git-coauthor
```

## Contributing

Contributions are welcome! Please submit a pull request or create an issue to discuss any changes you want to make.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.