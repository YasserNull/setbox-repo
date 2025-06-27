# SetBox Repository

Welcome to the **SetBox** repository.  
Here, you can contribute by creating your own modules and enhancing the user experience. Please follow the rules and instructions below.

## Rules

- All content inside module files **must be in English**
- The `id` must match the GitHub repository name
- Do **not** use any offensive or inappropriate language
- Modules must be **open-source** and licensed under **GPLv3**

## Module Instructions

Each module should contain **only three files**:

### 1. `module.prop`
Contains basic module information. Example:

```
id=battery-saver
name=Battery Saver
description=Enable battery saver mode
author=YasserYvY
version=v1.0.0
versionCode=1
repository=https://github.com/YasserYvY/battery-saver
```

### 2. `on`
This file contains commands to be executed **when the module is enabled**.  
Example:
```
secure doze_enabled 1
```

### 3. `off`
This file contains commands to be executed **when the module is disabled**.  
Example:
```
secure doze_enabled 0
```

#### Command Format (`on` and `off` files)

```
<type> <key> <value>
```

Available types:
- `system`
- `secure`
- `global`

## Repository Structure

Your module repository should follow this structure:

```
your-module-repo/
├── module.prop
├── on
└── off
```

## Visitor Counter Badge

You can add a badge to show how many users have viewed (downloaded) your module:

```markdown
### Visitors at SetBox
![Visitors at SetBox](https://visitor-badge.laobi.icu/badge?page_id=YasserYaY/setbox-repo)
```

## How to Submit Your Module

1. Create your module repository following the structure and rules above
2. Open an `Issue` in this repository explaining your module and include its link
3. If everything is valid, your module will be added to [SetBox](https://github.com/YasserNull/setbox) 