meteor-isolate-bug
==================
See live demo at http://meteor-isolate-bug.meteor.com

Initial commit is a clean slate installation of the todos example. 

The only set of changes can be viewed here. 
https://github.com/tonyxiao/meteor-isolate-bug/commit/c5b255948235a166e5115f51f9aac1176c16a4f6


To reproduce the bug, open http://meteor-isolate-bug.meteor.com in two separate browsers windows. Enter some text into the "should be presered, but isn't" text field, then edit the task below in a different browser tab. The text field is re-rendered (user input lost) despite the {{#isolate}} tag. 

It seems that this has something to do with the way {{#each}} interacts with {{#isolate}}. 
