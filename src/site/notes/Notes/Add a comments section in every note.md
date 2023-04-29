---
{"dg-publish":true,"permalink":"/notes/add-a-comments-section-in-every-note/","tags":["unpublish, compiled"]}
---


# Add a comments section in every note in Digital Garden

I make this static website using Obsidian plugin called [Digital Garden](https://dg-docs.ole.dev/). 
No comment section as default. I need to embed third-party 'app' . I use [Disqus](https://disqus.com/). 

## How?
1. Register Disqus account 
2. In setting, click Add Disqus To Site
![Pasted image 20230311180629.png](/img/user/Attachments/Pasted%20image%2020230311180629.png)
3. Scroll to the bottom, click GET STARTED
 ![Pasted image 20230311180733.png](/img/user/Attachments/Pasted%20image%2020230311180733.png)
4. Click I want to install Disqus on my site
![Pasted image 20230311180821.png](/img/user/Attachments/Pasted%20image%2020230311180821.png)
5. Enter your Website Name, chose Category, click Create Site

![Pasted image 20230311180939.png](/img/user/Attachments/Pasted%20image%2020230311180939.png)
6. On this window, click the bottom "I don't see my platform...."

![Pasted image 20230311181656.png](/img/user/Attachments/Pasted%20image%2020230311181656.png)

7. Copy this code 
![Pasted image 20230311181842.png](/img/user/Attachments/Pasted%20image%2020230311181842.png)

8. Make "comment.Njk" file in your github repo under this path "digital-garden/src/site/_includes/components/user/notes/footer". Paste the code. Mine looked like this
 ![Pasted image 20230311182205.png](/img/user/Attachments/Pasted%20image%2020230311182205.png)

9. Let Vercel rebuild the website
10. And now you have a comment section on your website.
![Pasted image 20230311182707.png](/img/user/Attachments/Pasted%20image%2020230311182707.png)




#### Linked notes

[[Notes/Preparing Obsidian Publish\|Preparing Obsidian Publish]]
[[Notes/ConvertKit\|ConvertKit]]
[[Notes/How to embed Newsletter on Obsidian\|How to embed Newsletter on Obsidian]]
