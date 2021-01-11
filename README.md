# As clean as a whistle

## About
Because short codes are great, but readable codes are better.

## Source File Basics
All Swift source file should end with .swift. The naming format should be name+type.swift. Before creating a new file, please check all existing file name on the project that may cause ambiguosity to the name of your new file, then change your new file name accordingly.

### Language
File name language should be in English, with exceptions of some Indonesian words that may cause confusion when translated to english/the name itself is a part of the feature name. Discuss with other devs about this issue.

### Abbreviations
Do not use abbreviations (like ViewController -> VC) to avoid confusion. As an example if we have `TableViewCell` and `TableViewController`, both of them would be shortened to `TVC` which is ambiguous and not good.

**Good**

`HomeViewController.swift`, `CheckoutViewController.swift`, `ClinicListTableViewCell.swift`

**Bad**

`HomeVC.swift`, `HistoryTableVC.swift` (Unclear wether it is ViewController or ViewCell), `PurchasedItemsCell.swift` (Unclear wether it is a CollectionViewCell or TableViewCell)


## Code Formatting
Always use camelCase

**Good**
``` swift
Code here
```

Bad
``` swift
Code here
```
### Variables
Variable name should be in English, with exceptions of some Indonesian words that may cause confusion when translated to english/the name itself is a part of the feature name. Discuss with other devs about this issue.

Avoid shortening variable names, always aim for readability.

**Good** 
``` Swift
var personName: String = ""
var phoneNumber: Int = ""
var personGender: String = ""
var personBloodType: String = ""
```

**Bad**
``` Swift
var name = ""
var number = ""
var gender = ""
var blood = ""
```

### Outlets
Name outlets with name+type
``` swift
@IBOutlet weak var transactionHistoryTableView: UITableView!
@IBOutlet weak var passengerNamelabel: UILabel!
@IBOutlet weak var passportImage: UIImage!
```


