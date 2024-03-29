---
{"dg-publish":true,"permalink":"/notes/how-to-embed-newsletter-on-obsidian/","tags":["publish, compiled"]}
---


# How to embed Newsletter on Obsidian

I use [[Notes/ConvertKit\|ConvertKit]] to manage my [[Notes/Newsletter\|Newsletter]]. 
Here are steps to embed it to your Obsidian notes:

1. Sign up to [[Notes/ConvertKit\|ConvertKit]]. The steps are self-explanatory.
2. In your Convertkit home page, go to  Grow>Landing Pages & Forms

![Screen Shot 2022-07-06 at 6.51.32.png](/img/user/Attachments/Screen%20Shot%202022-07-06%20at%206.51.32.png)

3. Click  + Create New > Landing Pages , and Choose your template of choice
![Screen Shot 2022-07-06 at 6.57.19.png](/img/user/Attachments/Screen%20Shot%202022-07-06%20at%206.57.19.png)

5. Edit the appearance as you pleased and click Publish
![Screen Shot 2022-07-06 at 6.59.33.png](/img/user/Attachments/Screen%20Shot%202022-07-06%20at%206.59.33.png)

6. Copy the URL for publication. 
![Screen Shot 2022-07-06 at 7.06.56.png](/img/user/Attachments/Screen%20Shot%202022-07-06%20at%207.06.56.png)

7. In your note in Obsidian, use iframe to embed the URL. See codes below and change the https://awesome-speaker-2973.ck.page/ea63c6e045 to your URL.

```
<iframe src="https://awesome-speaker-2973.ck.page/ea63c6e045" style="width:100%; height:400px; border:none; margin-top:-60px"></iframe>
```

8. Check in View mode. It supposed to look like this:
(well, below is not the Landing Page we just made. Its mine which I made previously )

<iframe src="https://awesome-speaker-2973.ck.page/ea63c6e045" style="width:100%; height:400px; border:none; margin-top:-60px"></iframe>

9. Now you can see the visitor from https://app.convertkit.com/forms

#### Linked notes
[[Notes/Newsletter\|Newsletter]]
[[Notes/ConvertKit\|ConvertKit]]
[[000_My Second Brain\|000_My Second Brain]]