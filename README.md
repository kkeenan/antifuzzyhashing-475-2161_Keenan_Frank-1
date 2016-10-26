Purpose:

Fuzzy hashing provides a comparison of two files whose content may only vary slightly.  Tools that provide such a service, like ssdeep or VirusTotal, are very helpful to forensic investigators as they can aid in finding potentially incriminating files.  However, an individual may wish to protect their files from such a technique.


Solution:

Our solution is a Windows command line utility that will serve as an anti-fuzzy hashing tool.  The tool will take a type of file (i.e. mp3) and perform a fuzzy hashing function on it.  Then, the tool will make small changes (In the case of an mp3 file, these changes could include slightly altering the pitch or adding in small pauses.) to the file that will result in the second fuzzy hashes to be completely different.