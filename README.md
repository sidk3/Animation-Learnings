# Animation Learnings - Y-Bot from Mixamo

## Project Overview:
This project is a simple demonstration of **basic animations** using a **Y-Bot** model imported from **Mixamo**. The bot features three primary animations:
- **Idle**: The bot stands still.
- **Walk**: The bot walks forward.
- **Run**: The bot runs forward.

The animations are controlled within Unity using the **Animator window** to set up transitions between different states, allowing the bot to smoothly switch between idle, walking, and running animations.

## Features:
- **Idle Animation**: The bot remains still when no movement is triggered.
- **Walking Animation**: The bot walks when a low movement input is detected.
- **Running Animation**: The bot runs when a higher movement input is detected.
- **Smooth Animation Transitions**: Transitions between the animations are controlled via Unity’s **Animator Controller**.

## Requirements:
- **Unity 2020.3 or higher**
- **Mixamo account** (for downloading the Y-Bot model and animations)
- **Basic understanding of Unity’s Animator window** and animation state machines.

## Getting Started:

### 1. Download the Y-Bot Model and Animations from Mixamo:
1. Visit [Mixamo](https://www.mixamo.com/).
2. Search for **"Y-Bot"** (or any character of your choice).
3. Choose the animations: **Idle**, **Walk**, and **Run**.
4. Download the model with the selected animations in the **FBX** format.

### 2. Set Up Your Unity Project:
1. Open **Unity Hub** and create a **3D** project.
2. Import the **Y-Bot model** (the FBX file you downloaded) into Unity:
   - Drag and drop the FBX file into the **Assets** folder in your Unity project.
3. Ensure the **Rig** type is set to **Humanoid** (in the import settings of the Y-Bot model).
4. Import all the animations (Idle, Walk, Run) associated with the Y-Bot.

### 3. Create and Set Up an Animator Controller:
1. Right-click in the **Assets** window, then select **Create > Animator Controller** and name it something like `YBot_Animator`.
2. Double-click the Animator Controller to open the **Animator window**.
3. Drag the **Idle**, **Walk**, and **Run** animations into the Animator window as separate **Animation States**.
4. Connect these animation states using **transitions**:
   - **Idle → Run → Walk → Idle** (for looping between the states).
   - You can adjust the **transition conditions** to control when each animation occurs (for example, using **Speed** or other parameters).
![Idle image](https://github.com/sidk3/Animation-Learnings/blob/main/Idle.png)
### 4. Assign the Animator Controller to the Y-Bot:
1. Select the Y-Bot in the **Hierarchy** window.
2. In the **Inspector**, find the **Animator** component.
3. Assign the **YBot_Animator Controller** to the Animator component.

![Running image](https://github.com/sidk3/Animation-Learnings/blob/main/Running.png)

### 5. Testing the Animation in Unity:
1. Press **Play** in Unity.
2. The Y-Bot will transition between the **Idle**, **Walk**, and **Run** animations based on the transitions you set up in the Animator.

> Note: Since there is no user input or custom code, the transitions between animations will occur automatically based on the default transitions you set in the Animator window. You can adjust the speed or conditions for each state transition for better control.

## How to Play:
1. Press **Play** in Unity to start the demo.
2. You can watch the Y-Bot transition between idle, walking, and running states based on the animation setup in the Animator.

## Credits:
- **Character**: Y-Bot from **Mixamo**
- **Game Engine**: **Unity**
- **Animations**: Mixamo's **Idle**, **Walk**, and **Run** animations
