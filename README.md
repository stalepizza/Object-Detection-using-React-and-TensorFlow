# Object Detection with React and TensorFlow.js

This project demonstrates real-time object detection in the browser using React, TensorFlow.js, and the COCO-SSD model. The application leverages the webcam feed to identify objects and displays bounding boxes around them. This implementation is inspired by [Nicolas Renotte's tutorials](https://www.youtube.com/c/NicolasRenotte).

## Features
- Real-time object detection using the COCO-SSD model.
- Integration with TensorFlow.js for browser-based machine learning.
- Clean and responsive UI with webcam and canvas elements.

## Technologies Used
- **React**: For building the user interface.
- **TensorFlow.js**: For loading and running the COCO-SSD model.
- **COCO-SSD Model**: Pre-trained model for object detection.
- **Webcam**: For capturing video input in real-time.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/object-detection-app.git
   cd object-detection-app
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open your browser and navigate to `http://localhost:3000`.

## File Structure
```
.
├── public
├── src
│   ├── App.js         # Main React component
│   ├── App.css        # Styling for the app
│   ├── utilities.js   # Utility functions like drawing bounding boxes
│   ├── index.js       # Entry point of the React app
│   └── assets         # Images or other assets (if needed)
├── package.json       # Project configuration and dependencies
└── README.md          # Documentation
```

## How It Works

1. **Load TensorFlow.js and COCO-SSD**:
   The app uses TensorFlow.js to load the COCO-SSD model. TensorFlow.js provides compatibility with browser environments, enabling machine learning directly in the client.

2. **Webcam Integration**:
   The app uses the `react-webcam` library to capture live video from the user's webcam.

3. **Object Detection**:
   The COCO-SSD model runs inference on the video feed to detect objects in real-time. Detected objects are drawn on a canvas overlay using bounding boxes and labels.

4. **Bounding Box Rendering**:
   The `drawRect` function in `utilities.js` handles rendering bounding boxes and object labels over the webcam feed.

## Usage

- Open the app in your browser.
- Grant permission to access the webcam.
- The app will display the webcam feed and detect objects in real-time.
- Detected objects will appear with bounding boxes and labels.

## Known Issues

- **Performance**: Detection might be slower on older devices or browsers without WebGL support.
- **Model Loading Error**: Ensure a stable internet connection for downloading the COCO-SSD model. If issues persist, consider hosting the model locally.

## Inspiration
This project was inspired by Nicolas Renotte's tutorials on machine learning and computer vision. Check out his [YouTube channel](https://www.youtube.com/c/NicolasRenotte) for more great content.

## License
This project is open-source and available under the [MIT License](LICENSE).

## Acknowledgments
- [TensorFlow.js](https://www.tensorflow.org/js): For making machine learning in the browser possible.
- [Nicolas Renotte](https://www.youtube.com/c/NicolasRenotte): For inspiring this project.

Feel free to contribute to this project or use it as a starting point for your own object detection application!

## Connect with Me
- **LinkedIn**: [Prisha Prakash](https://www.linkedin.com/in/prisha-prakash-950816297/)
- **Email**: prishaprakash9903@gmail.com
