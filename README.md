# VSCode Settings
A quick tutorial for myself.

* [C++](#C++)
* [Python](#Python)
* [Node.js](#Node.js)
* [Git](#Git)

## C++
1. Download VSCode
    [Click me](https://code.visualstudio.com/download)
    ![](https://i.imgur.com/373Aznl.png)

2. Install Extensions
    * C/C++
    ![](https://i.imgur.com/UC7BxvB.png)

    * C++ Intellisense
    ![](https://i.imgur.com/nlnJnOS.png)
3. Install MinGW
    * [Click me](https://sourceforge.net/projects/mingw/)
    ![](https://i.imgur.com/yL0qK9E.png)
    * Select **mingw32-gcc-g++ (bin)**, and then go to **All Packges** select **mingw32-gdb (bin)**.
    * Click **Installation** -> **Apply Change**

4. Set Environment Variables
    * Paste C:\MinGW\bin
    ![](https://i.imgur.com/Acon4lF.png)
    
5. Set folders for C++ program
    * Structure like this
    ![](https://i.imgur.com/szf53C0.png)
    
    * Download from [here](https://github.com/YuYuTW123/VSCode_Settings) or copy codes below
    
    **task.json**
    ```json=
    {
        "tasks": [
            {
                "type": "cppbuild",
                "label": "C/C++: g++.exe build active file",
                "command": "C:\\MinGW\\bin\\g++.exe",
                "args": [
                    "-fdiagnostics-color=always",
                    "-g",
                    "${file}",
                    "-o",
                    "${fileDirname}\\${fileBasenameNoExtension}.exe"
                ],
                "options": {
                    "cwd": "${fileDirname}"
                },
                "problemMatcher": [
                    "$gcc"
                ],
                "group": {
                    "kind": "build",
                    "isDefault": true
                },
                "detail": "Task generated by Debugger."
            }
        ],
        "version": "2.0.0"
    }
    ```
    
    **settings.json**
    ```json=
    {
        "files.associations": {
            "ostream": "cpp",
            "array": "cpp",
            "atomic": "cpp",
            "bit": "cpp",
            "*.tcc": "cpp",
            "cctype": "cpp",
            "clocale": "cpp",
            "cmath": "cpp",
            "compare": "cpp",
            "concepts": "cpp",
            "cstdarg": "cpp",
            "cstddef": "cpp",
            "cstdint": "cpp",
            "cstdio": "cpp",
            "cstdlib": "cpp",
            "cwchar": "cpp",
            "cwctype": "cpp",
            "deque": "cpp",
            "string": "cpp",
            "unordered_map": "cpp",
            "vector": "cpp",
            "exception": "cpp",
            "algorithm": "cpp",
            "functional": "cpp",
            "iterator": "cpp",
            "memory": "cpp",
            "memory_resource": "cpp",
            "numeric": "cpp",
            "random": "cpp",
            "string_view": "cpp",
            "system_error": "cpp",
            "tuple": "cpp",
            "type_traits": "cpp",
            "utility": "cpp",
            "initializer_list": "cpp",
            "iosfwd": "cpp",
            "iostream": "cpp",
            "istream": "cpp",
            "limits": "cpp",
            "new": "cpp",
            "numbers": "cpp",
            "stdexcept": "cpp",
            "streambuf": "cpp",
            "typeinfo": "cpp",
            "iomanip": "cpp"
        }
    }
    ```

6. Start Coding!!
    * Press **Ctrl+Shift+B** and it'll start build.
    ![](https://i.imgur.com/jFchpgA.png)
    * After building succeed, enter **./(Your_file_name).exe** it'll run the file.
    ![](https://i.imgur.com/eCAprOg.png)


## Python

1. Install Python
    * [Click me](https://www.python.org/)
    * Check if Python is installed in terminal.
    ![](https://i.imgur.com/RWg25oD.png)
    
    **Note.** There's a checkbox for adding Python to PATH. So basically we don't need to add Python to Environment Variables by ourselves.
    ![](https://i.imgur.com/3AikD5Q.png)

2. Set folders for Python program
    * Structure like this
    ![](https://i.imgur.com/pMP6gkw.png)

    * Download from [here](https://github.com/YuYuTW123/VSCode_Settings) or copy codes below

    **settings.json**
    ```json=
    {
        "python.pythonPath": "C:\\Users\\User_name\\AppData\\Local\\Programs\\Python\\Python39\\python.exe",
        "python.linting.enabled": true,
        "python.linting.pylintEnabled": true
    }

    ```
3. Install Python Extension
    ![](https://i.imgur.com/o6oWsr8.png)

4. Start Coding!!
    * Before executing the program, enter below codes in the terminal to install debugger.
    ```pip intall pylint```
    
    * Enter **python (Your_file_name).py** in the terminal to run the file.
    ![](https://i.imgur.com/UiMZGdP.png)
    
    
## Node.js

Install Node.js
[Click me](https://nodejs.org/en/)
    
**Note.** Same as Python, the Environment Variables is already set, there's no need to set it again.

## Git

Install Git
[Click me](https://git-scm.com/download/win)

**Note.** Same as Python and Node.js, the Environment Variables is already set, there's no need to set it again.
