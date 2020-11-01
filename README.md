WIP.

Investigation into LRS:
- Make a GET request to `https://lrswapi.campus.mcgill.ca/api/MediaRecordings/dto/<course_id>` where `course_id` can be obtained from the div tag `HF_CourseID` on mycourses. The header of the request must contain the bearer token associated with the current mycourses login session. The bearer token can be found in the tag `HF_JWT`.
- The response will be a JSON object. The sources key will be associated with a array of objects containing the LRSCDN m3u8 files. Copy the src link and add `.m3u8` to it
- Past this in as the first argument to `./download.sh`, with the second being the output destination and file.
    - e.g. ./download.sh `<src>.m3u8>` `~/Download/output.mp4`
