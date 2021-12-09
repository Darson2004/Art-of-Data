I worked with Elias, Bulyn, Claire, and Tuhin on this lab.
For the csv file, I thought a good way to create it was to use classes.
I created a large class that contained its init, str, and an attempt to 
begin a csv method.


However, I realized that not only was the class not the most efficient way
to create the csv, but that it was the slowest and most unnecessary amount
of code, given we could use API systems to request the information from the
online csv. 

```
import requests 
key = "ArtOfDataKEY123"
index = 0
payload = {'key': "ArtOfDataKEY123", 'idx': index}
response = requests.get("https://hm-cs.herokuapp.com"+"/socks", params=payload)
##We have gotten the request from the website and gave it our payload. Now
##the website is giving back the ok or not, determining whether it will give
##information.
while(response.ok):
   data = response.text
   index += 1
   payload = {'key': "ArtOfDataKEY123", 'idx': index}
   response = requests.get("https://hm-cs.herokuapp.com"+"/socks", params=payload)
   print(data)
```

From this question, I learned how to code API better, as this API code was
slightly different from the API code for just a website. We used a key this
time; I also thought we should have done index = 1, but that would leave out
the headers, so that's why its equal to 0.


The second question took the longest amount of time. While working with Bulyn,
we tried to do it with classes. However, because I stopped using classes from
the first question, I could no longer do it the way he did. I went back to
pseudocode and tried to do it using dictionaries and lists. I realized that
Elias did it the same way, and he helped me figure out the correct pseudocode
as well as teach me two new things I could add for the code to look better.

```
variation = {}
	for sock in data:
		Name = sock["Name"]
		Variation = sock["Variation"]
		if Name not in variation:
			variation[Name] = 0
		variation[Name] += 1

#Create the list now
	
maxName = []
	largest_variation = 1 #cheers to Elias for this

	for sock in variation:
		if variation[sock] > largest_variation:
		largest_variation = variation[sock]
		maxName = [] 
		maxName.append(sock)
	else if variation[sock] == largest_variation: #this adds the next names that have the same number of appearances in the csv
		biggest.append(sock) 

x = ", ".join(biggest) #also cheers Elias for this thing too
print("The socks with the most variations are " + x + ".")
```

We first create a dictionary to add all the socks and then a list for the most 
variations per sock. Elias taught me .join(biggest) and to use largest_variation.

From this question, I learned to use dictionaries and lists together, when we usually
separate the two.

In the second question, I worked with Elias again, this time creating a dictionary to
hold both color 1 and color 2. Elias taught me another piece of code, this time "continue"
If the color 1 and 2 were the same, we would continue or go past it. It was to make the
code look cleaner.

```
colors = {}
for sock in data:
    color1 = sock["Color 1"]
    color2 = sock["Color 2"]
    if color1 not in colors:
        colors[color1] = 0
    colors[color1] += 1
    if color2 not in colors:
        colors[color2] = 0
    elif color2 == color1:
        continue
    colors[color2] += 1

print(colors)
```
