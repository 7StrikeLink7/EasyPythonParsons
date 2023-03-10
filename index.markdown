---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Tutorial 
---
## Parsons Tutorial 
Problem:
Drag and re-arrange the blocks so to output: 

Hello!
This is a print statement.
The text in between the brackets get displayed to you.


<div id="0-sortableTrash" class="sortable-code"></div> 
<div id="0-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="0-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="0-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "print(“Hello!&quot;)\n" +
    "print(“This is a print statement.&quot;)\n" +
    "print(“The text in between the brackets get displayed to you.”)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "0-sortable",
    "max_wrong_lines": 0,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "0-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#0-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#0-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Topics:
[Outputs](./parsons/Outputs.html)
[Variables and Outputs](./parsons/Variables.html)
[Variables, Outputs, and Inputs](./parsons/Inputs.html)
[Maths Operators (input integers)](./parsons/Inputs.html)
[Random numbers](./parsons/Random.html)
[Strings and Casting](./parsons/Casting.html)
[Booleans](./parsons/Booleans.html)
[If](./parsons/If.html)
[If/Else](./parsons/Else.html)
[If/Elif/Else](./parsons/Elif.html)
[Nested Ifs](./parsons/NestedIf.html)
[For loops](./parsons/For.html)
[While loops](./parsons/While.html)
[Nested loops](./parsons/NestedLoops.html)
[Arrays/Lists](./parsons/Arrays.html)
[2D Lists](./parsons/2D.html)
[File handling](./parsons/Files.html)
[Subprograms(functions/procedures)](./parsons/Subprograms.html)
 

 
![image](https://user-images.githubusercontent.com/68385109/213919695-59481689-588f-4df1-8037-23c09f5bf6ac.png)

