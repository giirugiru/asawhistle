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
var phoneNumber = ""
var backgroundImage = ""
func fetchUserID()
```

**Bad Example**
```
var phoneNum = ""
var bgImg = ""
```

### Variables

**Good Example** 
``` Swift
var personName: String = ""
var phoneNumber: Int = ""
var personGender: String = ""
var personBloodType: String = ""
```

**Bad Example**
``` Swift
var name = ""
var number = ""
var gender = ""
var blood = ""
```

### Outlets
Name outlets with name+type. For example:
``` swift
@IBOutlet weak var transactionHistoryTableView: UITableView!
@IBOutlet weak var passengerNamelabel: UILabel!
@IBOutlet weak var passportImage: UIImage!
```

### Booleans
Give names to booleans starting with is, has, have, etc. For example `isSelected`, `hasOrdered`, `isUploading`



