# About
This little snippet is created to work with Joni Korpi's LessFramework and SASS language (http://sass-lang.com/).

The basic idea is that you often want to hide/display/expand to full width a certain block of text/image/element depends on the current resolutions of users' browsers. For example, you may want to expand your banner in the left column to full width on an iPhone screen but often want the object to return back to the left column for users with better screen size.

This is designed to work with LessFramework 3. As LessFramework 5 is under development, I'll wait until its release then update the code to accommodate with the newer version. In contrast to Joni's LessFramework3 where the 8 columns version is considered as the default resolution, I have decided to make the 3 columns version (target iPhone and mobile device) as the default version and delegates changes to other resolutions. As a matter of fact, you can compare the main.scss and lessframework3.css to see the difference. I believe it makes my life and probably your easier.

Check out http://JMango.net for a real life example. Try resizing the website slowly you will start to see blocks moving around/become hidden or take full width.

# File Structures
 /README - instruction
 /main.scss - The main base scss file, this is your central css file.
 /_ninja.scss - the core of Ninja Stealth :)
 /_reset.scss - it's written for generic purpose and is based on Blueprint's reset so I decide to include it here.
 /_colors.scss - put your colour variables in here.
 /_utility.scss - put your utility variables and blocks in here. Included as a bonus, not that vital.
 /lessframework3.css - The original lessframework3 file included for comparison with the main.scss. You can remove it from your production environment.
 
# How to
## Compile
By running this command.
sass --watch main.scss:main.css

And you should not be worry about other files that starts with underscore as they are automatically compiled by SASS and included to the final css file.
## Usage and examples
Check out the /examples folder.