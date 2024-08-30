
### File Organizer Script

#### Overview

This Python script is designed to streamline the process of organizing files within a directory by categorizing and moving them into specific folders based on their file extensions. It's a practical tool for anyone who deals with a cluttered workspace or frequently needs to sort files of various types. The script can handle a wide range of file formats, from images and videos to documents and archives, ensuring that your files are neatly organized and easy to find.

#### Key Features

1. **Comprehensive File Type Support**:
   - The script recognizes and organizes files into various categories, including:
     - **HTML Files**: `.html5`, `.html`, `.htm`, `.xhtml`
     - **Image Files**: `.jpeg`, `.jpg`, `.tiff`, `.gif`, `.bmp`, `.png`, `.svg`, `.heif`, `.psd`
     - **Video Files**: `.avi`, `.flv`, `.wmv`, `.mov`, `.mp4`, `.webm`, `.vob`, `.mng`, `.qt`, `.mpg`, `.mpeg`, `.3gp`
     - **Document Files**: `.oxps`, `.epub`, `.pages`, `.docx`, `.doc`, `.fdf`, `.ods`, `.odt`, `.pwi`, `.xsn`, `.xps`, `.dotx`, `.docm`, `.rvg`, `.rtf`, `.rtfd`, `.wpd`, `.xls`, `.xlsx`, `.ppt`, `.pptx`
     - **Archive Files**: `.a`, `.ar`, `.cpio`, `.iso`, `.tar`, `.gz`, `.rz`, `.7z`, `.dmg`, `.rar`, `.xar`, `.zip`
     - **Audio Files**: `.aac`, `.aa`, `.dvf`, `.m4a`, `.m4b`, `.m4p`, `.mp3`, `.msv`, `ogg`, `oga`, `.raw`, `.vox`, `.wav`, `.wma`
     - **Plain Text Files**: `.txt`, `.in`, `.out`
     - **PDF Files**: `.pdf`
     - **Python Scripts**: `.py`
     - **XML Files**: `.xml`
     - **Executable Files**: `.exe`
     - **Shell Scripts**: `.sh`

2. **Customizable Directory Structure**:
   - The directory structure is defined in the script, allowing you to easily modify or add new categories and associated file extensions. This flexibility makes it adaptable to various user needs and different types of projects.

3. **Efficient File Management**:
   - By automating the organization process, this script reduces the time and effort required to sort files manually. It ensures that your workspace remains clutter-free and that files are stored in their appropriate locations.

4. **User-Friendly Implementation**:
   - The script is simple to use: just place it in the directory you want to organize and run it. The script will automatically detect files and move them into the appropriate folders based on their extensions. 

5. **Extensible and Maintainable**:
   - Written in Python, the script is easy to understand and modify. The use of Python’s `os` and `pathlib` libraries makes it robust and reliable, while the clear structure of the code allows for straightforward maintenance and updates.

#### How It Works

1. **Directory Definition**:
   - The script starts by defining a dictionary (`DIRECTORIES`) that maps categories (e.g., `IMAGES`, `VIDEOS`) to a list of file extensions associated with those categories.

2. **File Mapping**:
   - A second dictionary (`FILE_FORMATS`) is generated, which maps each file extension to its corresponding directory. This allows for quick lookup and categorization of files.

3. **File Sorting**:
   - The script iterates through all files in the working directory. For each file, it checks its extension and determines which directory it belongs to. It then moves the file to the appropriate directory, creating the directory if it doesn't already exist.

4. **Custom Modifications**:
   - Users can easily modify the `DIRECTORIES` dictionary to add new file types or change existing categories. The script is designed to be adaptable to various organizational needs.

#### Use Cases

- **Personal File Organization**: Ideal for individuals who need to regularly organize a large number of files, such as photographers, video editors, writers, or developers.
- **Workplace Efficiency**: Can be used in professional settings where files are frequently exchanged and need to be organized systematically.
- **Project Management**: Useful for managing files within specific projects, ensuring that all resources are neatly categorized and easily accessible.

#### Getting Started

1. **Clone the Repository**:
   - Clone the GitHub repository to your local machine using the command:
     ```
     git clone https://github.com/yourusername/file-organizer.git
     ```

2. **Navigate to the Directory**:
   - Change to the directory containing the script:
     ```
     cd file-organizer
     ```

3. **Run the Script**:
   - Execute the script in the directory you want to organize:
     ```
     python organize.py
     ```

4. **Customize If Necessary**:
   - Modify the `DIRECTORIES` dictionary in the script if you need to handle additional file types or change the directory structure.

#### Future Enhancements

- **GUI Version**: Developing a graphical user interface to make the tool more accessible to non-programmers.
- **Scheduled Automation**: Adding functionality to run the script automatically at specified intervals.
- **Integration with Cloud Services**: Extending the script to organize files stored on cloud services like Google Drive or Dropbox.

