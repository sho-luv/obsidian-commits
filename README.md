# Obsidian Commits
![GitHub release)](https://img.shields.io/github/v/release/Darakah/obsidian-commits)
![GitHub all releases](https://img.shields.io/github/downloads/Darakah/obsidian-commits/total)

Track &amp; Review changes in obsidian vault or specified project. (Github like commit review)

## Example
<img width="841" alt="image" src="https://user-images.githubusercontent.com/1679089/224503771-f78a8afd-a82a-4ef3-9fa4-bb7c71f0e159.png">

<details>
  <summary>See Code used in example picture:</summary>
  
 ### Code used for example picture:
````
```commits-recents
project=/
divWith=7
divHeight=450
divAlign=left
topCommits=4
```
```commits-type
project=/
divWith=7
divHeight=450
divAlign=left
topCommits=5
```
```commits-daily
project=/
divWith=15
divHeight=400
divAlign=right
```
```commits-weekly
project=/
divWith=7
divHeight=400
divAlign=right
topCommits=5
```
````
</details>

<details>
  <summary>See Features:</summary>
## Features
- Track an obsidian vault / project's growth 
- Growth is divided into 4 categories: 
  - Create: Creating new notes
  - Expand: Increase size of already existing notes (threshold of change can be changed in settings, default 15% increase in size)
  - Link: Tag / Link a note (new connection)
  - Refactor: Restructuring includes deleting files, decreasing size of a file by a certain amount (default 15%), renaming, untagging and unlinking

- A unit of work is reffered to as a commit and is classified in one of the 4 categories above
- Show commits over hour of day
- Show commits over day of the week
- Show recent commits
- Track specific project or vault
- Custumize width / height / alignment / fill color / grid color of the different render blocks

**IMPORTANT: file size change / tag & link change are updated every 5 min!!**

  </details>
  
  <details>
  <summary>See Usage:</summary>
  
## Usage

  ### Blocks (visual displays)
---
There are four types of visual trackers aka (blocks) you can use. To display a specific block, you need to use its corresponding block ID. The available block IDs are:

- `commits-recents`
- `commits-type`
- `commits-weekly`
- `commits-daily`

Basic Block Inmplimentation Example:
````
```commits-recents
```
````

### Block Configurations
---
When using these blocks, you can set arguments to customize the display. Each argument should be on a separate line and should follow the syntax `argumentName=argumentValue`. For example, to set the width of a div container, you can use the argument `divWidth=50`, which sets the width to 50% of the note width.

The order in which the arguments are specified does not affect their behavior, and if an argument is not specified, the plugin will use its default value. However, it is important to note that not all available arguments work with every type of block. Here are the available arguments for this plugin:

- `project` - This argumentName is only configured to track the root by default which is shown as / in the setting of the Commits plugin. If you want to track something other than '/' root. You need to give the name of the (case sensitive) directory name you want to track in the settings. Then you can use this argumentName. 
- `topCommits` - Only used with the `commits-recents` block, and it displays links to the most recent # of affected documents, such as the last 4 deleted notes.
- You can assign color arguments using either color names (e.g., yellow, red) or the RGBA format (e.g., rgba(255, 97, 0, 0.95)). A helpful tool for selecting colors in the RGBA format is https://rgbacolorpicker.com/.
- `borderColor` - Change color of charts and graphs borders and text
- `gridColor` - Change the color of the grids used on charts
- `fillColor` - Change color of charts and graphs
- `divWidth` - Change width in percetage %
- `divHeight` - Change height in pixels
- `divAlign` - Change alignment to `center`, `left`, or `right`

### Block Arguments Examples
---
For the `commits-type`, `commits-weekly`, and `commits-daily` blocks, you can customize the following parameters:

Project Path: The default will track the whole vault from the root directory which is shown as /. If you want to track a project i.e. track a directory, use the settings tab of the plugin.

- Track project examples:
  - Track entire obsidian vault: `project=/`
  - Track everything in folder "Work" and below it: `project=Work`
  - Note the names are case sensitive.
- Div width in %, example `divWidth=50`
- Height in Pixels example `devHeight=300`
- Fill color example `fillColor=Coral`
- Fill color example `fillColor=rgba(255, 0, 0, 0.95)`
- Border color example `borderColor=Red`
- Grid color example `gridColor=rgba(255, 205, 92, 0.95)`
- Div container alignment, i.e., `center`, `right` or `left`.

For the commits-recents block, you can customize the following parameters:

Project Path: By default, only the whole vault is tracked and can be shown as /. If you want to track a new project, use the settings tab of the plugin.
- Top number of recent commits to show for each category example `topCommits=5`
- Div width in %, example `divWidth=50`
- Height in Pixels example `devHeight=300`
- Fill color example `fillColor=Coral`
- Div container alignment, i.e., `center`, `right` or `left`.

</details>

## Settings:
<img width="1101" alt="image" src="https://user-images.githubusercontent.com/1679089/224605873-0dd0fd19-247c-4041-b9c9-395d9e5ef949.png">

## Release Notes

### v0.2.2
- Code improvements & optimization

### v0.1.2
- Initial release


## Support

[![Github Sponsorship](https://raw.githubusercontent.com/Darakah/Darakah/e0fe245eaef23cb4a5f19fe9a09a9df0c0cdc8e1/icons/github_sponsor_btn.svg)](https://github.com/sponsors/Darakah) [<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="BuyMeACoffee" width="100">](https://www.buymeacoffee.com/darakah)\



