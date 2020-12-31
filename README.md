# CtrlSUpdated

Website: https://www.createchrisvk.in/ctrlS/

#Landing page: index.html

#Basic Feature: Real time shared file editing and project management teams

#Structure: You can be part of multiple teams -> Each team can have multiple projects -> Each project has multiple files, which can be edited in real time only by the members in the team You cannot be part of multiple teams with the same name, or create multiple projects of the same name in the same team. (However, different teams can have projects of the same name)

#Each project page has a chat window for discussion

#Unique feature: The app analyzes the contents of the project you're working on and generates a game based on the contents. The game can be played by the members, while working on the project. The games require at least 2 members of a project to be online on the project page

#The app includes 3 games so far

Word Association wordGamev1.php #Description: A game that generates a random keyword from all the project files' content (Removes stopwords and punctuations) and gives you 3s to enter the first word that comes to your mind when you see the word. Game over if you run out of time or type the same word twice. The other players can see your prompts and responses in real time

Draw the word draw.php #Description: A game where you have to draw an image to explain a word to your teammates. Again, the word is based on the project files' content.

StoryBoard getImgForStoryboard.php #Description: Gets random combinations of keywords from the project, performs a google image search on them, and shows you 3 random images from the search. Your task is to create a story out of these 3 images, which can be communicated via the chatbox.

The game files are embedded as iframes in newfile.php, which is the location for viewing project files, chat window or starting a game.

The new features are -

1. The app recommends -
  #Movies
  #TV Shows
  #Youtube Videos
  #Books
  Based on the content of the project being worked on (On the project page: newfile.php)

2. Users can now create and join common chat threads to meet new users with common interests (chatThreads.php)

3. We've built a chrome extension that
  #Checks if the user is active on any project page
  #If active, it adds a 'Sync' button at the top right corner of every website that the user visits
  #When this button is checked, all the content highlighted by the users get appended to a file called 'synced.txt' in the active project

  This is an easy way for all users to have all their research synced automatically in one place.

  #How to use the extension - 
    #Download the extension folder (ctrlS extension)
    #Open chrome://extensions in developer mode
    #Select 'Load Unpacked'
    #Choose the extension folder
    
  #Also, to test the extension with localhost, the extension assumes the app is in a folder called ctrlS (localhost/ctrlS/home.php)

*********PLEASE NOTE:**********
In order to make the recommendations, certain APIs were needed for the databases. Since an api key is sensitive, they have been replaced by "<YOUR API KEY>" in the files. Kindly generate your api key from the respective websites and replace it in the files.

The following files will need Api keys -
1. movies.php (api.themoviedb.org)
2. tvShows.php (api.themoviedb.org)
3. ytvids.php (Youtube v3 api)
