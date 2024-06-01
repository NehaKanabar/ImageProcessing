<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
  <h1 align="center">🖼️ Image Processor 🤖</h1>

  <p align="center">A Flask application which classifies images of sports personalities. 📸</p>

  <p align="center">
    <a href="#introduction">🎬 Introduction</a> •
    <a href="#installation">🛠️ Installation</a> •
    <a href="#usage">📸 Usage</a> •
    <a href="#api-endpoints">📡 API Endpoints</a> •
    <a href="#technologies-used">🛠️ Technologies Used</a> •
    <a href="#contributing">🤝 Contributing</a> 
  </p>

  ---

  <h2>🎬 Introduction</h2>

  <p>The Image Processor is a web application that uses machine learning to classify images of famous sports personalities like Lionel Messi, Maria Sharapova, Roger Federer, Serena Williams, and Virat Kohli. Upload an image, and the app will identify the sports person in the image with a probability score for each possible match. 🏃‍♂️🎾</p>

  <img src="https://github.com/NehaKanabar/ImageProcessing/assets/130577117/13e46ac9-cc94-4f34-b693-582ffee30521">

  <h2>🛠️ Installation</h2>

  <p>To run this Flask application locally, follow these steps:</p>

  <ol>
    <li>Clone this repository to your local machine.</li>
    <li>Install the required dependencies using <code>pip install -r requirements.txt</code>.</li>
    <li>Run the Flask server using <code>python server.py</code>.</li>
    <li>Access the application in your web browser at <code>http://localhost:5000</code>.</li>
  </ol>

  <h2>📸 Usage</h2>

  <p>Upload an Image:</p>
  <ul>
    <li>Drag and drop an image into the upload area or click to select a file. 🖱️</li>
  </ul>
  <p>Classify the Image:</p>
  <ul>
    <li>Click on the "Classify" button to start the classification process. 📊</li>
  </ul>
  <p>View Results:</p>
  <ul>
    <li>The app will display the detected sports personality and the probability scores for each possible match. 📸💬</li>
  </ul>

  <h2>📡 API Endpoints</h2>

  <h3>POST /classify_image</h3>

  <p>This endpoint is used to classify images based on facial features. 🧑‍🎨</p>

  <p><strong>Parameters:</strong></p>
  <ul>
    <li><strong>image_data:</strong> The base64-encoded image data of the sports personality to be classified. 🖼️</li>
  </ul>

  <p><strong>Response:</strong></p>
  <p>The response contains the classification results, including the detected sports personality, probability scores for each possible match, and a dictionary mapping class names to their corresponding numbers. 📝</p>

  <p>Example response:</p>
  <pre>
  <code>[
    {
      "class": "lionel_messi",
      "class_probability": [89.2, 4.5, 2.1, 1.8, 2.4],
      "class_dictionary": {
        "lionel_messi": 0,
        "maria_sharapova": 1,
        "roger_federer": 2,
        "serena_williams": 3,
        "virat_kohli": 4
      }
    }
  ]
  </code>
  </pre>

  <p><strong>Note:</strong> The <code>class_probability</code> array contains the probability scores for each class in percentage, and the <code>class_dictionary</code> provides the mapping of class names to their numerical representation. 🧾</p>

  <h2>🛠️ Technologies Used</h2>

  <ul>
    <li>Flask</li>
    <li>Python</li>
    <li>JavaScript</li>
    <li>HTML</li>
    <li>CSS</li>
  </ul>

  <h2>🤝Contributing</h2>

  <p>Join me in making the Image Processor even better! Whether it's fixing bugs, adding new features, or improving documentation, your contributions are highly appreciated. 🌟</p>

</body>
</html>
