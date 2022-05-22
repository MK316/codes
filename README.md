# codes lists and references

## 🎯 [Using Github files on Colab (copy to Colab)](https://github.com/MK316/codes/blob/main/Files_from_Github_to_Colab.ipynb)

```ruby
# copy a file from github
import os
url = "https://raw.githubusercontent.com/Youraccountname/repositoryname/main/foldername/filename.txt"
os.system("curl " + url + " > filename.txt")
```
```ruby
# read a text file in the server
file = open("filename.txt")
text = file.read().replace("\n", " ")
file.close()
```

```ruby
# write out a text file
file = open("filenametosave.txt", "w")
file.write(text)
file.close()
```


## 🎯 Github image link on Colab

1. Go to Github
2. Go to your Image
3. Copy the URL
4. Convert the URL in two steps: a. Change: /github.com/ to **raw.githubusercontent.com** b. **Remove "/blob/"** from the URL
5. Now in Colab's Text paste the edited URL inside the format: You will get an image displayed.
