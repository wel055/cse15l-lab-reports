# Lab Report 2
## Part 1
  __Code for ChatServer__
  ![Image](ChatServerCode.png)  
     
  __Screen shots of requests__
  ![Image](/add-message?s=Hello&user=jpolitz.png)  
     
  `/add-message?s=Hello&user=jpolitz`
     
  Methods Called:  
  `handleRequest(URI url)` is called by the server framework when a request is received.  
  Arguments and Values:  
  `url`: The URI object would have a string representation of `/add-message?s=Hello&user=jpolitz`.  
  Before the request, assuming chatHistory is empty, `chatHistory.toString()` would return an empty string.  
  Field Changes:  
  chatHistory would change from previous chat (in this case empty) to append jpolitz: `Hello\n`, resulting in `chatHistory.toString()` returning `jpolitz: Hello\n`.  
  
  ![Image](/add-message?s=How are you&user=yash.png)  
  
  `/add-message?s=How are you&user=yash`  

  Methods Called:  
  `handleRequest(URI url)` is called by the server framework when a request is received.  
  Arguments and Values:  
  `url`: The URI object would have a string representation of `/add-message?s=How are you&user=yash`.  
  Before this second request, `chatHistory.toString()` would return `jpolitz: Hello\n`.  
  Field Changes:  
  chatHistory would append `yash: How are you\n` to previous message.

  

  __2. ls__  
    ![Image](lsnoarg.png)  
      
     `ls`  
     
  Absolute path: /Users/wenxili/Desktop/UCSD/CSE 15L  
     
  The command ls with no argument shows all files in the current directory. I have three folders in CSE 15L: Commandcat Commanded Commandls. Therefore ls shows these three folders.  
     
  The output is not an error.  
