#!/bin/sh
# This is setup-hooks.sh

# Define where to clone the hooks repository
HOOKS_REPO_URL="https://github.com/your-organization/git-hooks-template.git"
HOOKS_DIR="$HOME/.git-templates/hooks"

# Clone the hooks repository
git clone $HOOKS_REPO_URL $HOOKS_DIR

# Set the template directory to include the hooks
git config --global init.templateDir "$HOME/.git-templates"

echo "Hooks template directory set to $HOME/.git-templates"
