# 624-PE01
Input:
The program receives inputs through two primary sources:
Code Input: The developer writes JavaScript/React Native code defining components (1 View, 3 Text) and styles (StyleSheet), including text content ("Sam Chung," "MSCS," "STC") and a yellow background.
Runtime Commands: The npx expo start --tunnel command triggers the development server and generates a QR code for device preview.
Process:
Bundling & Compilation: Expo CLI uses Metro Bundler to compile React Native code into executable JavaScript and native UI components.
Network Tunneling: The --tunnel flag establishes a public URL via Ngrok, enabling external access to the local server for mobile testing.
Layout Rendering: React Native’s layout engine calculates positioning (e.g., justifyContent: 'center') and applies styles to the components.
Output:
Mobile Interface: A screen with a yellow background displays three bold, centered text lines matching the input content.
Web Preview: Pressing "w" opens a browser version with identical styling.
Validation: The app dynamically updates via Expo’s Hot Module Reloading (HMR) when code changes, ensuring real-time feedback.
