my_first_php_work
=================
I have created a website for the field museum of Chicago. The requirement was to display information about their Sue exhibit and a running competition. Sue is the fossil of dinosaur which is placed as an exhibit at the Chicago Field Museum. Also there is a competition running to win a framed picture. 
I created two php pages- index.php and result.php. 
I displayed the show timings and its corresponding event room in the index page. There is a selectable side bar, which I downloaded from http://jqueryui.com, where I displayed options like ‘adopt a Museum’, ‘what to see?’ etc . I attached a footer and header to all the pages. 
I have displayed three images of sue in a special format where each image changes position on every page refresh.
 
For that I used the css float command. Also the pictures will be changing positions randomly at every refresh. I attained that by first creating a multi-dimensional array containing the name and source of the pictures and then used ‘shuffle’ command to shuffle the array randomly.   From this randomly shuffled array I retrieved each images using their index and displayed it along with its attribute.
 There is also a Lucky draw form which takes in name, competition code and a checkbox as inputs, which when submitted will be directed to the results.php page where I have done all the validations. 
In the results.php page I validated whether 
•	The user have entered name, competition code and checked the check box.
•	Otherwise an error message will be shown
•	If entered correctly I split the competition code into parts using ‘explode’ command separating it with blank space
•	Then I check whether the number of part is 3.
•	Else an error message will be shown
•	Then I checked whether the 1st two parts are numeric and the last part is alpha-numeric and also the length of part1=5, part2=3 and part3=5
•	Else an error message is displayed.
•	Now I check whether the part2, which is the code is equal to ‘333’
•	Then I display a message “congratulation” as it is the winning code
•	Else I displayed “We are sorry, but you have not won anything with the code:”
I have used POST as the action method so no sensitive data will be displayed in the url.
I have given option in the header to go back to the home page

