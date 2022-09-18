# ios-professional
My repository for learning iOS fundamentals in a concrete way

## How to start without storyboards

Go to video 14 in iOS Professional
Steps:
1. Delete Scene Delegate
2. Delete main.storyboard
3. Shift + command + F -> search main
4. Search main for the infoplist removal
5. Remove and then in info plist remove Application manifest completely
6. Get rid of everything inside App delegate class(all the functions inside it)

### Code Snippets(making it handy for us to store code in xcode)
7.  A code snippet for "no storyboard":
```
    var window: UIWindow?
    
    func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool {
        
        window = UIWindow(frame: UIScreen.main.bounds)
        window?.makeKeyAndVisible()
        window?.backgroundColor = .systemBackground
        window?.rootViewController = ViewController()
        
        return true
    }
```


