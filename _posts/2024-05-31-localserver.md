---
layout: post
title: How to Install Jekyll Static Website Generator on Ubuntu 20.04
date: 2024-05-31 00:00:00-0400
description: How to Install Jekyll Static Website Generator on Ubuntu 20.04
tags: Jekyll, ubuntu, local-server, website
categories: sample-posts
related_posts: false
giscus_comments: true
---


This note refers from this [Youtube tutorial](). Some details are a little bit different and I hope this can help you build up and debug your website or blog on your local server(You can also use Git to push your updated file to Github, but this would take a few minutes to see the actual update on your online web):

1.  Open a terminal(ignore the **conda** environment you already installed, just use the default environment)

    ![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su1.70a6dm7hjz.webp)
2.  ```shell
    sudo apt install make build-essential curl git tree -y
    ```
    
    ![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su2.6m3qmr16jq.webp)
3.  ```
    sudo apt install ruby ruby-dev -y
    ```
    
    ![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su3.4n7jwfavj5.webp)
4.  ```
    gedit ~/.bashrc
    ```

     Then you will open a file named .bashrc, go to the bottom of the file and then add these two lines on that:
    
    ```
    export GEM_HOME=$HOME/gems 
    ```
    
    ```
    export PATH=$HOME/gems/bin:$PATH
    ```
    
    ![](https://github.com/JackTony123/picx-images-hosting/raw/master/su4.839voip11x.webp)
    
    Then source your `.bashrc` file: 
    
    ```
    source ~/.bashrc
    ```
    
    



5. ```
   gem install jekyll bundler
   ```

   ![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su5.6pncknbaze.webp)
6. Then, install jerkII through 

   ```
   sudo apt install jekyll
   ```

   
7. Then, you can download the example web project from their official website to test whether your installation is successful.

   ```
   jekyll new jekyll.example.com
   ```

   ![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su6.8ojjazofo9.webp)
8. Then use tree 

   ```
   jekyll.example.com 
   ```

   to see the website project structure.
9. Go to the example project 

   ```
   cd jekyll.example.com
   ```

   , then run 

   ```
   bundle add webrick
   ```

    to install webrick.
10. Finally, you can run the example web project on your local server by running `jekyll serve --host=0.0.0.0`

    (Note: you may occur this problem as the picture shown below:

    ![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su7.5mnn9rva1d.webp)

No worry about that\~ Just close the terminal and then open a new terminal again in your project location to run the same command, then you will see:

![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su8.2obd69r31l.webp)

The website can been seen on your default browser as shown below:

![image](https://github.com/JackTony123/picx-images-hosting/raw/master/su9.7lju0464w2.webp)

-----------------------UPDATE----------------------------------

Sometimes when you may meet the problem like that:

![](https://github.com/JackTony123/picx-images-hosting/raw/master/prob_server.41xyyfpfsg.webp)

No worry about that, you can just change the input command like this:

```
bundle exec jekyll serve --host 0.0.0.0
```

Then the problem will be dealt with.
