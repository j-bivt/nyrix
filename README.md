# big update up and coming!!!
In this new update that is still a work in progress, 5 new things will be added.
- While Loop

- For Loop

- Lists

- Functions

> Here is some syntax examples below

> note: subject to change.
```
# make a list
list [ini] &myList "everything" "after" "is" "all" "added" "to" "the" "list."
# append to said list
list [app] &myList "you" "can" "append" "multiple" "things."
# extract value from list
list [ext] &myList 1 @extracted_value

# loops
mkfunc $myFunc (
  io t in "press [enter] to continue"
)
while 1 == 1 $myFunc
list [ini] &example 1 2 3 4 5 6 7 8 9 10
for i in &example $myFunc
```
# small update v0.2, if
Nothing much in this update, added **optional** indentation, example below.
```
if 1 == 5 {
  io t out "Example print." [d]
  if "hi" == "hi" {
    io t out "Another example print." [d]
  }  
} >>> {
  io t out "Even another example print" [d]
}
```
