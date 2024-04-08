# PocketSpace
My own vision on a simple microblogging social network. With a focus user expression.

## User page and timeline personalization
What I want to create here is a fusion between twitter and neocities: Users should be able to express themselves and their interests as long as they have the knowhow.
Every userpage would have a default version with your usual user info, but should you choose to use a custom landing page, the user gets to essentially have a custom static website.

## Custom Page sanitization
I'm not just going to let users write any html and javascript as they please, but instead limit it to safer components: 
- Raw HTML is mostly fine, but events and forms are veto'd (Except for onClick).
- There will be some custom HTML tags to easily put default site components where the user wants them. Some will be required, like the profile info card and the posts' timeline.
- Javascript code will only be allowed to use or alter USER variables, anything else will be only read. I'm still thinking how to achieve this, but if all else fails, I can just ban JS and let CSS be the main star of the show.
- CSS is already pretty safe, but I should find a way to prevent user CSS themes from interfering with the site's functions (Like overlaying a float element on top of the topbar to prevent navigation)

# User Posts
- Markdown support
- Colored text support
- In-browser editor to aid users that don't know MD by heart or plain don't have the necessary characters on their keyboard layout
- User can customize their own posts' font, font color (limited to darker tones)

## SharedSpaces!
Users can create a SharedSpace that functions as a topical gathering place for users with a forum, a chat box, and a landing page that can be customized too!
- Your SharedSpace will have its own NavBar, to which you can add custom URLs to send people to related resources, like a wiki or a dedicated site!

## Quality of life
- Light and darkmode auto-change custom user colors to their opposite luma value for readability. Users can also choose custom dark and light theme colors for their page and posts.
