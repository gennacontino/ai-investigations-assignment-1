# ai-investigations-assignment-1
Identifying similar face structure characteristics among Bollywood celebrities

In Bollywood films, actors dazzle on the big screen wearing deep red sarees and brilliant gold jewels. Just like in Western media, the most conventionally attractive actors are typically chosen to play big roles, creating beauty standards that some viewers strive for. 

I was curious to use face_recognition to identify face structure characteristics of celebrities to search for trends. While looking for data, I came across an image dataset of the top Bollywood actors specifically. I had heard of controversial beauty standards in India – particularly the trend of skin bleaching or skin whitening that has been criticized for being inextricably [tied to colorism]([url](https://www.vogue.in/beauty/content/the-movement-against-skin-whitening-products-what-you-need-to-know)) – so I thought a dataset of just Bollywood celebrities might prove interesting. I settled on this dataset to see if I could find other common facial structure characteristics that could give insight into what the Hindi-language film industry considers "beautiful."

To do this, I used the face_recognition library on Python to iterate through a folder of images of 35 different celebrities and pull out the face_landmarks for each celebrity. After exporting them into a DataFrame, I created a function to identify the minimum and maximum of X and Y coordinates for different facial features. I then exported the data to a CSV to pull out relevant features that I could use to calculate the width of the celebrities' nose bridges, nose tips, bottom lips and space between their eyes. 

To build this into a full story about Bollywood-created beauty standards, I would want to interview industry experts as well as Bollywood fans and people who live in India to get a better understanding of what is considered conventionally attractive, then see if the face_recognition results match up to what they say. If I find more diversity among the results, it could be a sign that the industry is becoming more inclusive. 

While I would have to dig deeper to make any real conclusions (I'd like to separate the images by gender and run the code on a larger dataset), a few trends did jump out at me from my results:

- Smaller lips, shorter nose bridges and less space between eyes are most common among the celebrity faces analyzed
- Nose tip width varies greatly
