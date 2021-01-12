# As clean as a whistle

## About
Because short codes are great, but readable codes are better.


## Source File Basics
All Swift source file should end with .swift. The naming format should be name+type.swift. Naming format should use PascalCase. For example: `HomeViewController.swift`. Before creating a new file, please check all existing file name on the project that may cause ambiguosity to the name of your new file, then change your new file name accordingly.

### Language
File name language should be in English, with exceptions of some Indonesian words that may cause confusion when translated to english/the name itself is a part of the feature name. Discuss with other devs about this issue.

### Abbreviations
Do not use abbreviations (like ViewController -> VC) to avoid confusion. As an example if we have `TableViewCell` and `TableViewController`, both of them would be shortened to `TVC` which is ambiguous and not good.

**Good Example**

`HomeViewController.swift`, `CheckoutViewController.swift`, `ClinicListTableViewCell.swift`

**Bad Example**

`HomeVC.swift`, `HistoryTableVC.swift` (Unclear wether it is ViewController or ViewCell), `PurchasedItemsCell.swift` (Unclear wether it is a CollectionViewCell or TableViewCell)


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
Naming should be in English, with exceptions of some Indonesian words that may cause confusion when translated to english/the name itself is a part of the feature name. Discuss with other devs about this issue.

### Abbreviations
Avoid using abbreviations or shortening. Spell them out even if they are long. With exceptions of abbreviations that are commonly used. For example `handphone -> HP` , `Identifier -> ID`, etc. But prioritize spelling them out.

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
**Example**
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
Name outlets with name+type. For example:
``` swift
@IBOutlet weak var transactionHistoryTableView: UITableView!
@IBOutlet weak var passengerNamelabel: UILabel!
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



















