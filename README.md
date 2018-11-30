# Retrasar tarea con SWIFT
Retrasa una tarea el tiempo deseado

```swift
DispatchQueue.main.asyncAfter(deadline: DispatchTime.now()+1){
  // Codigo a retrasar 1 segundo
}

// O

DispatchQueue.global(qos: .userInitiated).async {
  if let u = URL(string: url){

    DispatchQueue.main.async {
      let res = URLRequest(url: u)

      DispatchQueue.main.async {
        self.web.loadRequest(res)
      }
    }
  }
}
```
