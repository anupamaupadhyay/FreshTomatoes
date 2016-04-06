# FreshTomatoes entertainment.py
import media

toy_story= media.Movie("Toy",
  "life is beauti",
  "https://en.wikipedia.org/wiki/File:Toy_Story.jpg",
 "https://www.youtube.com/watch?v=azyK_k52R1w")

#print (toy_story.storyline)



avatar= media.Movie("Avatar","alien",".jpg","url")
#print (avatar.storyline)
#print toy_story.show_trailer()



bajirao=media.Movie("BAjirao Mastani",
  "History",
  "https://en.wikipedia.org/wiki/Bajirao_Mastani",
  "https://www.youtube.com/watch?v=eHOc-4D7MjY")

#print bajirao.show_trailer()


---------------------
#media.py
import webbrowser

class Movie():
    def __init__(self,movie_title,movie_storyline,poster_image,trailer_youtube):
        self.title= movie_title
        self.storyline= movie_storyline
        self.poster_image_url = poster_image
        self.trailer_youtube_url= trailer_youtube


#Each instance menthod takes first argument as 'init'
    def show_trailer(self):
        webbrowser.open(self.trailer_youtube_url)
        
        
  

