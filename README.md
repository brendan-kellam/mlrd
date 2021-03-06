mlrd
====
[![PyPI version shields.io](https://img.shields.io/pypi/v/mlrd.svg)](https://pypi.python.org/pypi/mlrd/)


A command line tool for downloading MyCourses lectures.

## Responsible use & copyright warning
> :warning: Before using this tool, read the [university's responsible IT use document](https://www.mcgill.ca/secretariat/files/secretariat/responsible-use-of-mcgill-it-policy-on-the.pdf).

> :warning: Do not share downloaded lectures without prior permission from the owner. Sharing without permission is a potential breach of the owner's copyright.

## Prerequisites
- [Python 3.8+](https://www.python.org/downloads/)
- [ffmpeg](https://ffmpeg.org/download.html)

## Usage
After installation, run the following command in your terminal:
```
mlrd <course_id> <output_dir> <auth_token>
```

This will download all lectures for the given course to your directory of choice. The `<course_id>` and `<auth_token>` can be found by:
1. navigating to desired course's lecture recording page on MyCourses.
2. right click > inspect.
3. ctrl/cmd + f and search for `HF_CourseId` and `HF_JWT`. The values of these elements correspond to the `<course_id>` and `<auth_token>`.