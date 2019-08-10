[slide]
# Live Session

[live-stream videoId="342590118" playerType="vimeo" /]

[slido id="5faavvrx" /]
[html]
   <style>  
    #sectionTracker{
     color: #ffa000;
    }
  </style>
  <script>
    window.onhashchange = function() { 
      let previouslySelectedElement = document.getElementById('sectionTracker');
      if(previouslySelectedElement){
         previouslySelectedElement.id = "";
      }
      let urlId = window.location.hash;
      let currElement = document.querySelector(`.lesson-navigation-section a.content-link[href="${urlId}"]`);
      console.log(currElement);
      currElement.id = "sectionTracker";
    }
  </script>
[/html]

[/slide]
