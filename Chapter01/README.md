# Lynda_iOS_GameDev_Swift3_SpriteKit

## 01. Introduction
### 01_01-Welcome.mp4
### 01_02-What you should know before watching.mp4
### 01_03-How to use the exercise files.mp4
## 02. Introduction to SpriteKit
### 02_01-Create a SpriteKit project.mp4
### 02_02-The SpriteKit Scene Editor.mp4
### 02_03-Add and modify sprites.mp4
### 02_04-Modify existing sprites in code.mp4
### 02_05-Create sprites in code.mp4
### 02_06-Custom scenes and custom classes.mp4
### 02_07-Transition between scenes.mp4
### 02_08-Understanding different scale models.mp4
### 02_09-Understanding parents and children.mp4
### 02_10-Remove a child from its parent.mp4
### 02_11-Change a childs parent.mp4

代码清单：GameScene.swift

```swift
override func didMove(to view: SKView) {
    let player:SKSpriteNode = self.childNode(withName: "player") as! SKSpriteNode
    let player2:SKSpriteNode = self.childNode(withName: "player2") as! SKSpriteNode
    let drone:SKSpriteNode = player.childNode(withName: "drone") as! SKSpriteNode
    
    // drone.removeFromParent()
    // player2.addChild(drone)
    drone.move(toParent: player2)
    drone.position = CGPoint(x: -45, y: -45)
}

```
## 03. Add Physics
### 03_01-Add physics properties to sprites.mp4
### 03_02-Work with gravity.mp4
### 03_03-Use forces and impulses.mp4
### 03_04-Spawn physics objects from a scene file.mp4
### 03_05-Detect collisions.mp4
### 03_06-Bit coding fundamentals.mp4
### 03_07-Use bitmasks.mp4
### 03_08-Collision and contact masks.mp4
### 03_09-Respond to collisions.mp4
### 03_10-User data and collision handling.mp4
## 04. Work with Particle Effects
### 04_01-Apply particle effects.mp4
### 04_02-Load particles with code.mp4
## 05. Work with Actions
### 05_01-Create actions in a scene file.mp4
### 05_02-Create actions with code.mp4
### 05_03-Action sequences.mp4
### 05_04-Stop a running action.mp4
### 05_05-Frame animations.mp4
### 05_06-Frame animations with code.mp4
## 06. Work with Audio
### 06_01-Sound effects.mp4
### 06_02-Play background music.mp4
### 06_03-Preload sounds.mp4
## 07. Additional Features
### 07_01-Physics fields.mp4
### 07_02-Cameras.mp4
### 07_03-Lights.mp4
### 07_04-Optimization techniques.mp4
## 08. Conclusion
### 08_01-Next steps.mp4
