# File Naming Conventions

Using unique naming conventions for different file types might sound a bit complex, but given the variations in purpose and maintenance among different files, this approach makes sense. 

For instance, with PDF files primarily intended for finalized publishing, incorporating version numbers and dates into the naming convention can facilitate easy tracking of different versions. On the other hand, for Markdown files that are often subject to continuous updates and can be tracked for text changes through version control tools like Git, it's possible to omit version numbers and dates in naming, retaining only the file's subject as the name.

Therefore, considering how they're used and managed, I've sorted the files into two categories: 

- Text-based files such as Markdown and JSON, and 
- Binary files like Word or PDF. 

Each category has its own specific naming conventions.

## Text-based files

- Keep file names in lowercase letters.
- Use hyphens instead of underscores to separate words.
- Limit file names to standard ASCII alphanumeric characters.
- Avoid using generic page names like `document1.html`.

For example: `naming-style.md`

## Binary files

In principle, all status information[^1] such as version number, document status and confidentiality level should already be visible from the file names. The following syntax must be observed:

[^1]: It does not apply to OPLs, logs and reports that are continually updated. These files should be archived regularly. 

### Date

- Date format is `YYMMDD`, alternatively `YYYYMMDD`

### Subject

- Create meaningful but brief names
- Recommendation: maximum 15 characters
- Use underscores to separate
- Avoid using spaces, dots and special characters (& or ? or !)

### Status

- A capital `D` for "draft"
- A `Ri` for "released internally" 
- A `Re` for "released externally"
- A `N` for "invalid" if the content of the document or template is no longer valid and may no longer be used

### Version

- Prefix a [semantic version](https://semver.org/) with a capital `V`

The above elements shall be grouped together as follows: `<Date>_<Subject>_<Version><Status>.<File_Extension>`

For example: `20230815_Naming_Style_V0.0.1D.docx`

## Learn more

- [File Naming Conventions | Data Management](https://datamanagement.hms.harvard.edu/plan-design/file-naming-conventions)
- [Filenames and file types  |  Google developer documentation style guide](https://developers.google.com/style/filenames)

