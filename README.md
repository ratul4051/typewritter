# typewritter
Step 1: Add the Typed.js Library to Your Site
Go to your WordPress Dashboard.
Navigate to Appearance > Theme File Editor (or wherever you manage your custom code like Wp code).
Add the following code inside the <head> section of your theme’s header file (header.php) to include the Typed.js library via CDN or in the header footer section of code snippets.

<script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>

Step 2: Create the HTML for the Typing Animation

Decide where you want the typing animation to appear (e.g., in your main header or an introductory section).
Go to the editor for the page where you want to add the typing animation.
Add an HTML block and paste this code, adjusting the text around it as needed:

<h1>Hi, I'm <span id="typed"></span></h1>

Step 3: Add the Typed.js Initialization Script
After adding the HTML, you’ll need to add the JavaScript to initialize the animation. You can do this directly in the Custom HTML or Custom JavaScript section (if your theme or page builder supports it), or place it in the <footer.php> file in Theme File Editor.

Here’s the initialization code:

<script>
  var options = {
    strings: ["a WordPress Developer", "a Web Designer", "a Content Creator"],
    typeSpeed: 50,      // Speed at which each letter appears
    backSpeed: 30,      // Speed at which each letter is erased
    backDelay: 2000,    // Pause before typing again
    loop: true          // Repeat animation
  };

  var typed = new Typed("#typed", options);
</script>

