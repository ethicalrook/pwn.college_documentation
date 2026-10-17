# [Path traversal]

**Platform:** [pwn.college]  
**Topic:** [Path Traversal]

## 1. Goal
Read `/flag` outside the intended web directory.
ss
## 2. What I Did
curl commands
Tried to access the files of the server

```bash
curl --path-as-is http://challenge.localhost/data/../../../flag
```

## 3. What Happened
I noticed that we can there is no authentication in accessing the server files.


## 4. Why It Worked
The command worked because there were no authentication or authorization while accessing the files threw the servers, so by just doing .. what uses to travel threw directories went outside the server folder and the flag was in the other directory so I found it 

## 5. What I Learned
- Path traversal
- We can access the directories and files of server from web page if the restrictions is not there

## 6. Key Takeaway
[Path traversal is very critical vulnerability and can reveal the confidential information about the server.]