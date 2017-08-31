# xcode-snippets
Handy code snippets used in day to day programming and fast prototyping.

## Adding Snippets in Xcode:
You can clone the complete project in ```~/Library/Developer/Xcode/UserData/```

OR

Clone/Download the project on your machine and paste the .codesnippets file in ```~/Library/Developer/Xcode/UserData/CodeSnippets/```

## Examples
* **Temporary Label**

Adds a temporary label at the center of the viewcontroller's view.

Shortcut: `templabel`

Context: Code Expression

Code:
```swift
let label = UILabel()
        label.translatesAutoresizingMaskIntoConstraints = false
        label.text = String(describing: "text")
        self.view.addSubview(label)
        self.view.addConstraint(NSLayoutConstraint(item: label, attribute: .centerX, relatedBy: .equal, toItem: self.view, attribute: .centerX, multiplier: 1.0, constant: 0.0))
        self.view.addConstraint(NSLayoutConstraint(item: label, attribute: .centerY, relatedBy: .equal, toItem: self.view, attribute: .centerY, multiplier: 1.0, constant: 0.0))
```

* **IBOutlet**

Shortcut: `iboutletsnippet`

Context: Class Implementation

Code:
```swift
@IBOutlet var titleLabel: UILabel!
```

* **IBAction**

Shortcut: `ibaction`

Context: Class Implementation

Code:
```swift
@IBAction func cancel(_ sender: AnyObject) {
      // function body
    }
```

* **Vertical Constraint**

Shortcut: `vertical-constraint`

Context: Code Expression

Code:
```swift
NSLayoutConstraint.constraints(withVisualFormat:"V:|[view]|", options: NSLayoutFormatOptions(rawValue: 0), metrics: nil, views: ["view": view])
```

* **Horizontal Constraint**

Shortcut: `horizontal-constraint`

Context: Code Expression

Code:
```swift
NSLayoutConstraint.constraints(withVisualFormat:"H:|[view]|", options: NSLayoutFormatOptions(rawValue: 0), metrics: nil, views: ["view": view])
```

* **Color**

Shortcut: `color`

Context: Code Expression

Code:
```swift
UIColor(red: float/256.0, green: float/256.0, blue: float/256.0, alpha: 1.0)
```

* **Code Blocks**

Shortcut: `codeblocks`

Context: Class Implementation

Code:
```swift
   //MARK: - Override Functions
    
    //MARK: - IBActions
    
    //MARK: - Other Functions
```

* **Center-X Constraint**

Shortcut: `centerx`

Context: Code Expression

Code:
```swift
NSLayoutConstraint(item: view, attribute: .centerX, relatedBy: .equal, toItem: related_view, attribute: .centerX, multiplier: 1.0, constant: 0.0)
```

* **Center-Y Constraint**

Shortcut: `centery`

Context: Code Expression

Code:
```swift
NSLayoutConstraint(item: view, attribute: .centerY, relatedBy: .equal, toItem: related_view, attribute: .centerY, multiplier: 1.0, constant: 0.0)
```

* **Equal Width Constraint**

Shortcut: `equal-width`

Context: Code Expression

Code:
```swift
NSLayoutConstraint(item: AnyObject, attribute: .width, relatedBy: .equal, toItem: AnyObject?, attribute: .width, multiplier: 1.0, constant: 0.0)
```

## Authors

* **Hassan Ahmed Khan** - [iHAK](https://github.com/ihak)

