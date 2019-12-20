---
title: 【warning】whose-view-is-not-in-the-window-hierarchy
categories:
  - swift 随手记
id: 1536223524
---

一般弹窗无法弹窗的话，修改弹窗的调用位置，放在界面加载之后
```
    override func viewDidAppear(_ animated: Bool) {
        super.viewDidAppear(true)
        
            let alertController:UIAlertController = UIAlertController(title: "无法定位",message: "修改定位设置",preferredStyle: .alert)
            
            let OKAction = UIAlertAction(title: "OK", style: .default) { (action) in
                // ...
            }
            alertController.addAction(OKAction)
            self.present(alertController, animated: true, completion: nil)
    }
```


