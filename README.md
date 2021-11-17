# YouTube-Video-Download-In-Python




from pytube import YouTube


url = "https://www.youtube.com/watch?v=iqr7JDGppm0"



yvd = YouTube(url)         #yvd= variable



print("=========Title==========")



print(yvd.title)


print("============== Description===================")



print(yvd.description)


print("================rating===============")



print(yvd.rating)



print("===============thumbnail Images Link==============")



print(yvd.thumbnail_url)




print("=======YouTube Video Download==========")




for stream in yvd.streams:
    b = yvd.streams.get_highest_resolution()   #variable
    b.download()
      
