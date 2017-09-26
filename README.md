# Code-Project
Uploading, accessing and downloading cloud objects

# The purpose of this repository is to: 

Provide access to the location of shared objects

Provide sample code for accessing these objects

Provide the contents of the JSON object being used as a sample

For the purposes of transparency, the original source .txt file is provided

For the purpose of demonstrating JSON objects, the orginal source file was completely rewritten in JSON format

For the purpose of demonstrating what the entire output of the curl read command is, the curltest.out file is provided

# The Public REST Endpoint for the file is:

https://storage.googleapis.com/mike-triska-bucket/Michael_Triska_Resume_August2017.txt

# The Public REST Endpoint for the JSON object is:

https://storage.googleapis.com/mike-triska-bucket/triska-resume.json

# Curl Command Syntax to download the file:

curl -o testfile.txt https://storage.googleapis.com/mike-triska-bucket/Michael_Triska_Resume.txt

To test if the file is valid use an editor like MacOS TextEdit

# Curl Command Syntax to download the JSON object:

curl -o curltest.out -H "Content-Type: application/json" -X GET https://storage.googleapis.com/mike-triska-bucket/triska-resume.json

# Test if the object contains valid data in JSON format:

 grep -i "label" curltest.out                               
 
 "label": "Systems Architect",
