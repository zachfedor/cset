After completing the first course, how would I rate myself, and what are some things I want to do differently in the next course? As far as understanding the concepts and
completing the projects, I think I did pretty well. One thing I would like to improve on is participation. I think I could have done better with exploring new ideas, instead
of just doing what I had to.

What is the difference between objects and arrays? In the weresquirrel example, each entry in the journal is an object that has two properties: events, and squirrel. Properties
in an object aren't identified by the order in which they are listed in the object, but by their key - events, and squirrel. Each of these properties contain a value. The
squirrel property simply contains a boolean: whether he turned into a squirrel that day or not. The events property contains an array that contains everything that he did that
day. The values that are stored in an array are not identified by a key, but by the index of that value. FE: `["Hello", "world"]`. `"Hello"` is at index 0, and `"world"` is at
index 1. Every journal entry object is stored in an array called journal. Now the journal array contains every entry object in order, and each entry is identified by it's index.

The reason that `journal` is an array and not an object, is that not each entry needs it's own key. All that was needed was the list of entries. The reason that the entries are
objects is that each entry had to have certain characteristics. `squirrel` should contain a boolean, and `events` should hold an array. In my Choose Your Own
Adventure game, I could have created a "player" object whose properties were name, health, and amount of money. This would have made the code a bit more readable and more
organized.
