# CtrlSUpdated

The initial version of this app is at https://github.com/hridizaroy/CtrlS

Website: http://www.ctrlscollab.co

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

********ALSO NOTE:************
The website is currently hosted on an http server, and therefore the extension cannot be used with the website at the moment. It will be ready for use once the site is hosted on an https server. Kindly test it with localhost until then.
