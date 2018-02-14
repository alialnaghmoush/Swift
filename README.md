# UIKitPro: FrameWork By Ali AlNaghmoush
## This FrameWork contains:
- UIColor Pro
- UIAnchor Pro
---
# UIColor Pro
### UIColor Pro include most Google Color grades are as follows: <p>(50 - 100 - 200 - 300 - 400 - 500 - 600 - 700 - 800 - 900)</p>
### More Info About Google Color: https://material.io/guidelines/style/color.html

![red](https://user-images.githubusercontent.com/22422080/36191285-64a28f60-116d-11e8-92b1-a8a15c91beae.png)
![pink](https://user-images.githubusercontent.com/22422080/36191282-6318896a-116d-11e8-9f10-dcd2922c6aec.png)
![purple](https://user-images.githubusercontent.com/22422080/36191281-616c91ec-116d-11e8-9589-290dbbcd3ea4.png)
![deeppurple](https://user-images.githubusercontent.com/22422080/36191280-5f6260f2-116d-11e8-83c1-da9320e51e28.png)
![indigo](https://user-images.githubusercontent.com/22422080/36191275-5b4eb358-116d-11e8-873b-90fa5d930f9f.png)
![blue](https://user-images.githubusercontent.com/22422080/36191274-597139d4-116d-11e8-9b85-86e4884ba0e4.png)
![lightblue](https://user-images.githubusercontent.com/22422080/36191272-5799cb9e-116d-11e8-838d-4295b563ac0e.png)
![cyan](https://user-images.githubusercontent.com/22422080/36191268-55be0af6-116d-11e8-8fc6-a7005544f9f5.png)
![teal](https://user-images.githubusercontent.com/22422080/36191264-53d20c7e-116d-11e8-81c6-ed067e4541bb.png)
![green](https://user-images.githubusercontent.com/22422080/36191263-51e07072-116d-11e8-9451-efac409bff46.png)
![lightgreen](https://user-images.githubusercontent.com/22422080/36191259-4f25d4c6-116d-11e8-9560-adc3c2ed1fce.png)
![lime](https://user-images.githubusercontent.com/22422080/36191255-4d3a74fa-116d-11e8-8764-873d0805acfb.png)
![yellow](https://user-images.githubusercontent.com/22422080/36191254-4b60c710-116d-11e8-982c-cfa9988165eb.png)
![amber](https://user-images.githubusercontent.com/22422080/36191250-48d8cab0-116d-11e8-8645-d87d09335f44.png)
![orange](https://user-images.githubusercontent.com/22422080/36191247-467da1f0-116d-11e8-95d3-296421606cb6.png)
![deeporange](https://user-images.githubusercontent.com/22422080/36191243-4482d8d4-116d-11e8-93a5-dd13417f845f.png)
![brown](https://user-images.githubusercontent.com/22422080/36191239-40b513de-116d-11e8-92c8-325359939bd0.png)
![gray](https://user-images.githubusercontent.com/22422080/36191237-3ec0d194-116d-11e8-9aa2-6ccdda03879f.png)
![bluegray](https://user-images.githubusercontent.com/22422080/36191234-3c7d1604-116d-11e8-8a52-9979811fd501.png)

## How to use thes UIColor Pro library Google Colors Or Other future
### In the beginning,SetUp UIKitPro in Your project, and the library should be called in the file where the library code will be used as follows:
```
import UIKitPro
```

- First we call || `UIColor`
- Secondly we write G, to call all Google colors in the library || `UIColor.G`
- Thirdly, we write the name of the color after the letter G directly without any distance || `UIColor.GRed`
- Finally, we write the number of grades we want || `UIColor.GRed500`
- Congratulations, Enjoy With Google Color

## More examples
```
let gRedColor = UIColor.GRed500
let gDeepPurpleColor = UIColor.GDeepPurple700
let gLightGreenColor = UIColor.GLightGreen500

view.backgroundColor = UIColor.GYellow700
```
## The color library will not stop here will expand in the future.

---
---
---

# UIAnchor Pro
### UIAnchorPro Easy and powerful control in Swift
![aps00](https://user-images.githubusercontent.com/22422080/36202063-5ab09d1e-1193-11e8-843c-49b22bc5e5b4.png)
### The normal way of Anchor work in Swift Ex:

```
    ...

    func setupNavBar() {
        
        // Build Subview ===============================
        view.addSubview(topBar)
        topBar.translatesAutoresizingMaskIntoConstraints = false
        
        //Now Start Anchor Point normal way ===============================
        topBar.heightAnchor.constraint(equalToConstant: 91).isActive = true
        topBar.topAnchor.constraint(equalTo: view.topAnchor, constant: -1).isActive = true
        topBar.leadingAnchor.constraint(equalTo: view.leadingAnchor, constant: -1).isActive = true
        topBar.trailingAnchor.constraint(equalTo: view.trailingAnchor, constant: 1).isActive = true 
    }
    
    ...
    
```
```
    ...
    
    func setupRightBar() {
        
        // Build Subview ===============================
        view.addSubview(rightBar)
        rightBar.translatesAutoresizingMaskIntoConstraints = false
        
        //Now Start Anchor Point normal way ===============================
        topBar.heightAnchor.constraint(equalToConstant: 201).isActive = true
        topBar.topAnchor.constraint(equalTo: topBar.bottomAnchor, constant: 0).isActive = true
        topBar.bottomAnchor.constraint(equalTo: view.bottomAnchor, constant: 1).isActive = true
        topBar.trailingAnchor.constraint(equalTo: view.trailingAnchor, constant: 1).isActive = true 
    }
    
    ...
    
```
## With UIAnchorPro System
### You do not need to write each time this code || `Ex.translatesAutoresizingMaskIntoConstraints = false`
### You do not need to write each time a new line to know a certain Anchor || `topAnchor، bottomAnchor، leadingAnchor،trailingAnchor`
### You do not need to write each time a new line anchor || `isActive = true`

### Just write Anchor || `ex.anchor(...)`
### and chose One

![aps0](https://user-images.githubusercontent.com/22422080/36198521-e66e16b2-1187-11e8-8ad7-58fb0476e6ab.png)
### If you want anchor all Edges write:
```
        ex.anchor(view: view)
```
### If you want anchor all Edges With Padding write:
```
        ex.anchor(TLTBtop: view.topAnchor,
                  leading: view.leadingAnchor,
                 trailing: view.trailingAnchor,
                   bottom: view.bottomAnchor,
               paddingTop: 10, paddingLeading: 10, paddingTrailing: 10, paddingBottom: 10)
```
### Now we know how to use UIAnchorPro
### To select the appropriate anchor, the abbreviation of each Function is defined

- anchor(TLTBtop... || `Top, Leading, Trailing, Bottom`
- anchor(TLTtop... || `Top, Leading, Trailing`
- anchor(BLTbottom... || `Bottom, Leading, Trailing`
- anchor(TBLtop... || `Top, Bottom, Leading`
- anchor(TBTtop... || `Top, Bottom, Trailing`
- anchor(TBtop... || `Top, Bottom`
- anchor(LTtop... || `Leading, Trailing`
----------------------------------
- anchor(top... || `Top`
- anchor(bottom... || `Bottom`
- anchor(leading... || `Leading`
- anchor(trailing... || `Trailing`
----------------------------------
- anchor(height... || `Height`
- anchor(width... || `Width`
----------------------------------

## How to use thes library
### In the beginning,SetUp UIKitPro in Your project, and the library should be called in the file where the library code will be used as follows:
```
import UIKitPro
```
![aps1](https://user-images.githubusercontent.com/22422080/36198525-e9808be6-1187-11e8-83ea-1ba391fc5c8f.png)
```
        ex.anchor(TLTtop: view.topAnchor,
                  leading: view.leadingAnchor,
                 trailing: view.trailingAnchor,
               paddingTop: 10, paddingLeading: 10, paddingTrailing: 10)
```
```
        ex.anchor(BLTbottom: view.bottomAnchor,
                  leading: view.leadingAnchor,
                 trailing: view.trailingAnchor,
               paddingBottom: 10, paddingLeading: 10, paddingTrailing: 10)
```
![aps2](https://user-images.githubusercontent.com/22422080/36198528-ebc489de-1187-11e8-80e1-d5e78e23e5b2.png)
```
        ex.anchor(TBLtop: view.topAnchor,
                  bottom: view.bottomAnchor,
                  leading: view.leadingAnchor,
               paddingTop: 10, paddingBottom: 10, paddingLeading: 10)
```
```
        ex.anchor(TBTtop: view.topAnchor,
                  bottom: view.bottomAnchor,
                trailing: view.trailingAnchor,
              paddingTop: 10, paddingBottom: 10, paddingTrailing: 10)
```
![aps3](https://user-images.githubusercontent.com/22422080/36198534-edf90ebe-1187-11e8-86f7-1cbfba183eb3.png)
```
        ex.anchor(TBtop: view.topAnchor,
                 bottom: view.bottomAnchor,
             paddingTop: 10, paddingBottom: 10)
```
```
        ex.anchor(LTleading: view.leadingAnchor,
                   trailing: view.trailingAnchor,
             paddingLeading: 10, paddingTrailing: 10)
```
![aps4](https://user-images.githubusercontent.com/22422080/36198542-f0124a8a-1187-11e8-89f3-0f26afeadce2.png)
```
        ex.anchor(top: view.topAnchor, paddingTop: 10)
```
```
        ex.anchor(bottom: view.bottomAnchor, paddingBottom: 10)
```
![aps5](https://user-images.githubusercontent.com/22422080/36198556-f32ca508-1187-11e8-898f-d6908f20be24.png)
```
        ex.anchor(leading: view.leadingAnchor, paddingLeading: 10)
```
```
        ex.anchor(trailing: view.trailingAnchor, paddingTrailing: 10)
```
![aps6](https://user-images.githubusercontent.com/22422080/36198559-f5b8174e-1187-11e8-9c62-0b19db5ba469.png)
```
        ex.anchor(height: 100)
```
```
        ex.anchor(width: 100)
```

## Wait for the next developments
