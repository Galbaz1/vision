# Interactive Hand Gesture Physics Playground

## Quick Overview
An interactive web application that combines hand gesture recognition with physics-based interactions. Users can manipulate floating blocks with their hands in real-time, creating an engaging and intuitive interface where virtual objects respond to natural hand movements.

## Detailed Description

### Core Features
- **Real-time Hand Tracking**: Uses MediaPipe Hands for accurate hand landmark detection
- **Physics Engine Integration**: Implements Matter.js for realistic physics simulations
- **Multi-Hand Support**: Tracks up to two hands simultaneously
- **Interactive Objects**: 10 physics-enabled blocks with letters spelling "AIBUILDERS"
- **Gesture Recognition**: Pinch gestures for grabbing and manipulating objects
- **Visual Feedback**: Dynamic indicators for hand tracking and gesture detection

### Technical Implementation
1. **Hand Tracking System**
   - MediaPipe Hands API for real-time hand landmark detection
   - Camera feed processing with mirrored display
   - 21-point hand landmark tracking per hand

2. **Physics Engine**
   - Matter.js for physics simulation
   - Custom gravity and collision settings
   - Boundary system with invisible walls
   - Natural physics properties for objects (friction, restitution, etc.)

3. **Gesture System**
   - Pinch detection using thumb and index finger positions
   - Distance-based object selection
   - Spring constraints for natural object manipulation
   - Smooth transition handling for grab/release actions

4. **Visual Elements**
   - Animated title with gradient effects
   - Loading indicators and gesture feedback
   - Hand landmark visualization
   - Physics object styling with shadows and transitions

### User Interface
- Mirrored camera feed with semi-transparent overlay
- Visual indicators for pinch gestures
- Status messages for system state
- Colorful interactive blocks with letter labels
- Smooth animations and transitions

### Browser Compatibility
- Works in modern browsers supporting:
  - WebGL
  - MediaStream API
  - Canvas API
  - Modern CSS features

### Dependencies
- MediaPipe Hands
- Matter.js Physics Engine
- Anime.js
- TailwindCSS
- DaisyUI

### Performance Considerations
- Optimized physics calculations
- Efficient hand tracking with confidence thresholds
- Smooth visual updates with requestAnimationFrame
- Automatic cleanup and boundary checking

### Usage
1. Allow camera access when prompted
2. Show your hands to the camera
3. Use pinch gestures to grab and move the floating blocks
4. Interact with multiple blocks using both hands
5. Objects will respond to physics when released

This project demonstrates the potential of combining gesture recognition with physics simulations to create intuitive and engaging web-based interactions.