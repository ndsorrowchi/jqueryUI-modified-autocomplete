Hi,

Thank you for viewing this assignment. I have done it yesterday in my spare-time, but I wanted to make it more dynamic like github or twitter so I spent some time upgrading what I had done.

This auto-complete is done by JQuery but originally it has many disadvantages that I didn't like, so I found how to change the width as well as the pop-up position.

If you need me write the auto-complete myself from bottom-up, I would write it based on a <div>, which contains a <ul> element whose <li> childs contains selected results. Then I would write onclick() handlers for each list-item to remember the selected result and hide and delete the <div>. Then I need to write the function to make dynamically create the list <div> and show it in an absolute position and it's pretty much done. Please tell me if you want me to write it bottom-up since I still have one day left and that time is alsmost enough for me to finish it. Also, I cna configure the regular expression to make it exact match for what users just typed.

In order to get the position of the caret in the textarea, I used this(https://github.com/component/textarea-caret-position)
which is also used by github themselves for their stuff. This is for poping up the select list only at the caret spot. I get the coordinates of the caret, and the bounding rectangle of the textarea, the scroll information of the textarea, and calculate pop-up absolute position. Since the JQuery autocomplete already has a way to config pop up position(given the percentiles), I calcualte the percentiles and make it look good.

Thanks.

References:

JQuery UI- http://jqueryui.com/
textarea-caret-position: https://github.com/component/textarea-caret-position
bootstrap css: http://getbootstrap.com/