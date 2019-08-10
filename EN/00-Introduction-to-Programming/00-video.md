[slide]
# Training Session

[vimeo-video videoId="342590118" /]
[html]
<!-- 
Override scrolbar with webkit.
Won`t work in Firefox or IE/Edge
-->
<style>/* width */
::-webkit-scrollbar {
  width: 7px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1; 
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #888; 
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555; 
}</style>

<style>
  
</style>
[/html]

[html]
<!--
Section tracker script
-->
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
