## 03. Add Physics
### 03_01-Add physics properties to sprites.mp4

- add two color sprite to scene
- move one two the bottom
- change another sprite's color to blue
- change all sprite's Physics Definition -> Body Type to [Bounding rectangle]
- unchecked the red color sprites's properties [Dynamic],[Allows Rotaion],[Affected By Gravity]  

### 03_02-Work with gravity.mp4
### 03_03-Use forces and impulses.mp4

- 加载后向左移动
```swift
override func update(_ currentTime: TimeInterval) {
    // Called before each frame is rendered
    platform?.physicsBody?.applyForce(CGVector(dx: -30, dy: 0))
    //platform?.physicsBody?.velocity
}
```

- 点击屏幕，小人垂直向上跳跃
```swift
func touchDown(atPoint pos : CGPoint) {
    jump()
}
    
func jump() {
    // 修改图片
    guy?.texture = SKTexture(imageNamed: "guy_2")
    // 垂直向上跳500点
    guy?.physicsBody?.applyImpulse(CGVector(dx: 0, dy: 500))
}
```
### 03_04-Spawn physics objects from a scene file.mp4
### 03_05-Detect collisions.mp4
### 03_06-Bit coding fundamentals.mp4
### 03_07-Use bitmasks.mp4
### 03_08-Collision and contact masks.mp4
### 03_09-Respond to collisions.mp4
### 03_10-User data and collision handling.mp4

