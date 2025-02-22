## 04 - Control Flow

This is the order in which you command different actions/fucntions to happen within your project. Think of it like a flow diagram: 

![alt text](https://blog.knockknockstuff.com/wp-content/uploads/2013/07/Dilemmas_Social_ONLINE_vert31.jpg "Logo Title Text 1")

By querying what state the programme is at - there can be multiple outcomes. There are different ways of controlling the flow of your project. 

### if
Will probably be the most common of all the control flow commands you will use. You simply ask 'if' a condition has been met or happened yet.  

### else
An 'else' most commonly follows an 'if'. In the diagram above the 'else' is the lines that break up the YES and NO response. 

This provides an alternative action option for exmaple:

    ```swift

        if thereIsSomethingHere {
            YES doThis 
            } else {
            NO doSomethingDifferent 
            }  

        }
    ```    

### guard 
Guard statements are used to unwrap optionals and they provide alternate solution for conditional unwrapping. So it is a more secure version of an if statement becuase:
1. It has to be true 
2. It has to be followed by else 

### let
As discussed in the fundamentals notes a 'let' is a constant value 

## Combining these commands: 

### if let 
Simply asking if a constant exists

### guard let
More secure way of asking if a constant is true - as with a guard - it MUST BE TRUE

## Loops
Uses an array (list) of items. The command then filters through the list and the outcome is a value from that list. The list can be of any type for example: dictionaries, strings, intagers etc. 

### For In 
Loops through an arrary (list). It looks for a specific value within an specific array. For example: 

    ```swift 

        let names = ["Grace", "Kyle", "Ellen", "John"]
        
        for name in names {
            print("Hello, \(name)!")
        }
    

    ```
