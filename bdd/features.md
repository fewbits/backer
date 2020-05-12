# Backer - BDD - Features

## Feature: Create new Shell Script

**As**: a Shell Script user
**I want**: to be able to easily create a decent Shell Script
**So**: I don't need to always manually create a Shell Script and worry about what it needs to have

___

**Scenario**: New Shell Script successfully created
**Given**: The user has `backer` properly installed
**And**: There's no Shell Script called "my-shell-script" in the currend path
**When**: The user types `backer create my-shell-script`
**Then**: A new Shell Script called "my-shell-script" is created in the current path based on a well designed template/skelethon

**Scenario**: Shell Script with same name already exists
**Given**: The user has `backer` properly installed
**And**: There's a Shell Script called "my-shell-script" in the currend path
**When**: The user types `backer create my-shell-script`
**Then**:  The system notices that a Shell Script called "my-shell-script" already exists in the current path and fails saying `Error: a Shell Script called "my-shell-script" already exists`