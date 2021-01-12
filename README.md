# As clean as a whistle

## About
Because short codes are great, but readable codes are better.


## Source File Basics
All Swift source file should end with _.swift_. The naming format should be _name+type.swift_. Naming format should use PascalCase. For example: `HomeViewController.swift`. Before creating a new file, please check all existing file name on the project that may cause ambiguosity to the name of your new file, then change your new file name accordingly.

### Language
File name language should be in English, with exceptions of some Indonesian words that may cause confusion when translated to English/the name itself is a part of the feature name. Discuss with other devs about this issue.

### Abbreviations
Do not use abbreviations (like _ViewController_ -> _VC_) to avoid confusion. As an example if we have `TableViewCell` and `TableViewController`, both of them would be shortened to `TVC` which is ambiguous and not good.

**Good Example**

`HomeViewController.swift`, `CheckoutViewController.swift`, `ClinicListTableViewCell.swift`

**Bad Example**

`HomeVC.swift`, `HistoryTableVC.swift` (Unclear wether it is _ViewController_ or _ViewCell_), `PurchasedItemsCell.swift` (Unclear wether it is a _CollectionViewCell_ or _TableViewCell_)


## Code Formatting
Use PascalCase for types and protocols. Other than that, use camelCase.

**Good Example**
``` swift
Code here
```

**Bad Example**
``` swift
Code here
```

### Language
Naming should be in English, with exceptions of some Indonesian words that may cause confusion when translated to English/the name itself is a part of the feature name. Discuss with other devs about this issue.

### Abbreviations
Avoid using abbreviations or shortening. Spell them out even if they are long. With exceptions of abbreviations that are commonly used, for example _handphone_ -> _HP_ , _Identifier_ -> _ID_, etc. But always prioritize spelling them out.

**Good Example**
```
var phoneNumber = "02177189"
var backgroundImage = "apple.jpg"
func fetchUserID(){
}
```

**Bad Example**
```
var phoneNum = "02177189"
var bgImg = "apple.jpg"
```

### Variables
No need to specify data types if it can be easily identified, unless it is necessary.

**From**
``` swift
var name: String = "Kevin"
```
**To**
``` swift
var name = "Kevin"
```

Clarity is key. Be spesific and detailed when naming variables so other developer knows its definition and usage. Avoid using letters like `x`, `y`, `i`, or general/common words like `data`, `num`, `index`, `error`, thay may cause ambiguity or collide with other built in variables.

**Good Example** 
``` Swift
var personName = "Kevin"
var phoneNumber = "082110653234"
var personGender = "Male"
var personBloodType = "AB"
```

**Bad Example**
``` Swift
var name = "Kevin"
var num = 082110653234
var gender = "Male"
var blood = "AB"
```
These are not particularly bad, but it is highly suggested to have detailed variable names.

### Outlets
Name outlets with _name+type_.

**Example**
``` swift
@IBOutlet weak var transactionHistoryTableView: UITableView!
@IBOutlet weak var passengerNameLabel: UILabel!
@IBOutlet weak var passportImage: UIImage!
```

### Booleans
Give names to boolean variables starting with _is_, _has_, _have_, etc. For example `isSelected`, `hasOrdered`, `isUploading`.

### Braces

**Good Example**
``` swift
if user.isHappy {
  print("I am happy")
} else {
  print("I am not happy")
}
```

**Bad Example**
``` swift
if user.isHappy 
{
  print("I am happy")
} 
else 
{
  print("I am not happy")
}

// OR

if user.isHappy
{print("I am happy")} 
else
{print("I am not happy")}
```

### Colons
Colons should always have one trailing space but no leading space.

**Example**
``` swift
var heroes: [Hero] = []
```

### Operators
Operators should always have one leading and trailing space.

**Example**
``` swift
name = "Kevin"
age = 10

if name == "Kevin" && age < 17 {
  print("Kevin is young")
}
```

### Tuple, Array, Dictionary literals
Add trailing whitespace after comma. Parameter lists also applies this rule.

**Good Example**
``` swift
let numbers = [1, 2, 3]
```

**Bad Example**
``` swift
let numbers = [1,2,3]
let moreNumbers = [1 , 2 , 3]
```



### Functions
You don't need to specify the return type if the return value is void.

**From**
``` swift
func fetchData() -> Void {

}
```
**To**
``` swift
func fetchData(){

}

```

If you have multiple parameters, you can put each parameter on a new line for better readability.

**Example**
``` swift
func getRecord(
  patientName: String,
  patientDOB: String,
  patientAge: Int,
  patientBloodType: String,
  treatmentType: String,
  treatmentDate: String
){

}
```

## Code Organizing
There is no correct order of types, variables, functions, and any other components in a source file. Order may vary regardless of the content itself. What important is that each file and type uses some logical order which can be easily explained and understandable by the developers. Avoid "Chronological by date added" ordering. Instead, use `// MARK:` or `// MARK: -` comments to provide descriptions for that order or code grouping.

**Example**
``` swift
class MovieRatingViewController: UITableViewController {

  // MARK: - View controller lifecycle methods

  override func viewDidLoad() {
    // ...
  }

  override func viewWillAppear(_ animated: Bool) {
    // ...
  }

  // MARK: - Movie rating manipulation methods

  @objc private func ratingStarWasTapped(_ sender: UIButton?) {
    // ...
  }

  @objc private func criticReviewWasTapped(_ sender: UIButton?) {
    // ...
  }
}
```

### Protocols

**From**
``` swift
class MyViewController: UIViewController, UITableViewDataSource, UIScrollViewDelegate {
  // all methods
}
```

**To**
``` swift
class MyViewController: UIViewController {
  // class stuff here
}
 
// MARK: - UITableViewDataSource
extension MyViewController: UITableViewDataSource {
  // table view data source methods
}
 
// MARK: - UIScrollViewDelegate
extension MyViewController: UIScrollViewDelegate {
  // scroll view delegate methods
}
```

















