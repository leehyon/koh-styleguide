# Directory Naming Conventions

Maintaining a consistent and organized directory structure is essential for efficient data management. Below are examples of naming conventions I currently use for my directories.

## Windows

Use the following format to name a Windows directory:

- Avoid spaces and special characters in directory names. By default, Windows file systems are not case-sensitive
- Use **underscores** to separate words, such as `Project_Reports`

### Project directories

Basic rules for the structuring of project folders (unless otherwise specified by a tool etc.) are as follows: 

- Folders are numbered at the top level with a 2-digit number
- The number-letter combination is followed by an underscore and a short text without spaces (< 32 characters)

```
├───00_Config 
│   ├───01_Env_Setup  
│   ├───02_Tools  
│   └───09_Templates  
├───10_General  
│   └───11_MoM  
├───20_Project_Info   
├───80_Lessons_Learned  
└───90_Temp
```

## Linux and macOS

- Use lowercase letters for directory names. This helps with case sensitivity in Linux file systems
- Use **hyphens** to separate words in directory names, such as `marketing-campaigns`, it's generally more common to use hyphens

### $HOME top level directories

```
archive: obvious
documents: obvious
downloads: obvious
public: shared directory, network-accessible
self: obvious
work: obvious
```

## Learn more

- [How I organize my home directory | Alexandre de Verteuil](https://alexandre.deverteuil.net/post/organize-home-directory/)

