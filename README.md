# EmptyTableViewPlaceholder  
A simple extension to UITableview allows the caller to display a placeholder if the table datasource is empty.

###   
**Usage:**

1.  Add the ```UITableView+Extensions.swift``` file to your project directory (Drag and Drop)
2.  Simply, in your desired ViewController, just add this condition in your numberOfRows function to check your datasource and display the placeholder in case it is empty

```plaintext
if dataSourceArray.count == 0 {      
      tableView.setEmptyView(title: "No Accounts Found", message: "Your accounts will appear here.", messageImage: #imageLiteral(resourceName: "Add_Your_Image_Name_Here"))
        }else {
            tableView.restore()     
        }
}
```
