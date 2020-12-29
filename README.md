# SupportDocs: DataSource
This branch is where SupportDocs gets its data! You can add, edit, and delete documents here. For usage instructions, check out the `README`'s [usage](https://github.com/aheze/SupportDocs#using-the-github-repo) section in the main branch.

## Data Source JSON URL
<a href="https://raw.githubusercontent.com/stevenkellner/StrafenSupport/DataSource/_data/supportdocs_datasource.json">https://raw.githubusercontent.com/stevenkellner/StrafenSupport/DataSource/_data/supportdocs_datasource.json</a>

<details>
<summary><strong>Show examples</strong></summary>

<hr>

### SwiftUI
```swift
struct SwiftUIExampleView_MinimalCode: View {
    let dataSource = URL(string: "https://raw.githubusercontent.com/stevenkellner/StrafenSupport/DataSource/_data/supportdocs_datasource.json")!
    @State var supportDocsPresented = false
    
    var body: some View {
        Button("Present SupportDocs from SwiftUI!") { supportDocsPresented = true }
        .sheet(isPresented: $supportDocsPresented, content: {
            SupportDocsView(dataSource: dataSource, isPresented: $supportDocsPresented)
        })
    }
}
```

### UIKit
```swift
class UIKitExampleController_MinimalCode: UIViewController {
    /**
    Connect this inside the storyboard.
    
    This is just for demo purposes, so it's not connected yet.
    */
    @IBAction func presentButtonPressed(_ sender: Any) {
        let dataSource = URL(string: "https://raw.githubusercontent.com/stevenkellner/StrafenSupport/DataSource/_data/supportdocs_datasource.json")!
    
        let supportDocsViewController = SupportDocsViewController(dataSource: dataSource)
        self.present(supportDocsViewController, animated: true, completion: nil)
    }
}
```

<hr>

</details>

## Table of Contents
- [404 Page](https://stevenkellner.github.io/StrafenSupport/404) (SupportDocs Integrated File) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/StrafenSupport/404.md))
- [Abmelden Anderer Erzwingen](https://stevenkellner.github.io/StrafenSupport/Settings/ForceSignOutSettings) (settings3) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/Settings/ForceSignOutSettings.md))
- [Allgemeine Einstellungen](https://stevenkellner.github.io/StrafenSupport/Settings/GeneralSettings) (settings) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/Settings/GeneralSettings.md))
- [Allgemeines](https://stevenkellner.github.io/StrafenSupport/General) (general) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/StrafenSupport/General.md))
- [Anmelden / Registrieren](https://stevenkellner.github.io/StrafenSupport/LogIn-SignIn) (logIn-signIn) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/StrafenSupport/LogIn-SignIn.md))
- [Person Hinzufügen](https://stevenkellner.github.io/StrafenSupport/PersonActions/AddPerson) (person1) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/PersonActions/AddPerson.md))
- [Person Löschen](https://stevenkellner.github.io/StrafenSupport/PersonActions/DeletePerson) (person3) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/PersonActions/DeletePerson.md))
- [Person Ändern](https://stevenkellner.github.io/StrafenSupport/PersonActions/UpdatePerson) (person2) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/PersonActions/UpdatePerson.md))
- [Strafe Hinzufügen](https://stevenkellner.github.io/StrafenSupport/FineActions/AddFine) (fine1) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/FineActions/AddFine.md))
- [Strafe Löschen](https://stevenkellner.github.io/StrafenSupport/FineActions/DeleteFine) (fine3) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/FineActions/DeleteFine.md))
- [Strafe Ändern](https://stevenkellner.github.io/StrafenSupport/FineActions/UpdateFine) (fine2) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/FineActions/UpdateFine.md))
- [Strafen Teilen](https://stevenkellner.github.io/StrafenSupport/Settings/ShareFinesSettings) (settings2) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/Settings/ShareFinesSettings.md))
- [Verzugszinsen](https://stevenkellner.github.io/StrafenSupport/Settings/LatePaymentInterestSettings) (settings1) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/Settings/LatePaymentInterestSettings.md))
- [Vorlage Hinzufügen](https://stevenkellner.github.io/StrafenSupport/ReasonActions/AddReason) (reason1) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/ReasonActions/AddReason.md))
- [Vorlage Löschen](https://stevenkellner.github.io/StrafenSupport/ReasonActions/DeleteReason) (reason3) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/ReasonActions/DeleteReason.md))
- [Vorlage Ändern](https://stevenkellner.github.io/StrafenSupport/ReasonActions/UpdateReason) (reason2) ([edit](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/ReasonActions/UpdateReason.md))


## Notes
- Your changes make take up to five minutes to deploy. You can track the deployment progress [here](https://github.com/stevenkellner/StrafenSupport/deployments/activity_log?environment=github-pages).
- Do **not** update this file (`README.md`) directly. Your changes will be overriden the next time you push (the GitHub Action will regenerate this file). Instead, update the file in [`_scripts/README.md`](https://github.com/stevenkellner/StrafenSupport/edit/DataSource/_scripts/README.md). 