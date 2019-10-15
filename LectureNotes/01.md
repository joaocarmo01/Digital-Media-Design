**How do you see creativity?**

A process where people put ideas into practice, using the tools available to them.
I believe that it could be a group process.

**What is the significance of the problem for digital media design?**

A problem is what allows for employment in the world of design. A client has a problem, therefore needing to employ a designer/problem solver in a creative and strategic way.

**What is the key to working effectively (individually and collaboratively)?**

First, manage the stress, organize and set a goal (short goal).
The problem needs to be laid out, come up with various solutions, then find the most fitting solution.

**What is design about?**

I believe that design can be seen as a creative way to solve problems, which is usually interactive to an audience. 

**What are your aspirations to studying digital media?**

I would like to understand coding at various levels, so I can produce media for myself and others.
As well as become a multi-skilled individual, and learning how to solve problems.

**How will you make the most of studying Digital Media Design?**

I will try to develop my problem-solving skills as well as my ability to define a problem clearly.
Develop my technological skills, and become more flexible as an individual.

High Low Game:
 I was to some level scared, as I had no experience in coding. However, I was very curious as I am keen to learn and become skilled in this creative industry. Furthermore, I was impressed with how little time it took to produce a working game, but I am aware that in the real world it is more complicated.

```swift
import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var ScoreLabel: UILabel!
    
    @IBOutlet weak var TargetLabel: UILabel!
    
    var score = 0
    var target = 0
    var newTarget = 0
    
    override func viewDidLoad() {
        super.viewDidLoad()

        print("hello world")
        
    }

    @IBAction func HigherGuess(_ sender: Any) {
    generateNumber()
        if newTarget > target {
            correctGuess()
        } else {
            wrongGuess()
        }
    }
    
    @IBAction func GuessLower(_ sender: Any) {
   generateNumber()
          if newTarget < target {
              correctGuess()
          } else {
              wrongGuess()
        }
    }
  
    func generateNumber() {
        newTarget = Int.random(in: 0...100)
        }
    func correctGuess() {
       
        score += 1
        target = newTarget
        ScoreLabel.text = "Score: \(score)"
        TargetLabel.text = "\(target)"
    }
    func wrongGuess() {
        score = 0
        target = 0
        newTarget = 0
        ScoreLabel.text = "Score: \(score)"
               TargetLabel.text = "\(target)"
        
        
    }
    

}


```

