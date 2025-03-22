# Smart Pokédex: First Generation Pokémon Classifier

The Smart Pokédex is a web application designed to povide information of all the pokemon and classify the first 151 (Generation 1). It uses **TensorFlow** for image recognition, **SQLite** for data management, and **Streamlit** for a user-friendly interface. The project also includes a Convolutional Neural Network (CNN) trained on Pokémon images to classify them accurately.


## Features

- **Image Recognition**: Classifies Pokémon images using a trained CNN model.
- **Pokémon Information**: Displays detailed information about each Pokémon, including stats, types, abilities, and more.
- **User-Friendly Interface**: Built with Streamlit for an intuitive and interactive experience.
- **Database Management**: Uses SQLite to store and manage Pokémon data efficiently.


## Technologies Used

- **TensorFlow**: For building and training the CNN model for image classification.
- **SQLite**: For storing and querying Pokémon data.
- **Streamlit**: For creating the web application interface.
- **Pandas**: For data manipulation and preprocessing.
- **BeautifulSoup**: For web scraping Pokémon data.
- **Matplotlib**: For visualizing training results and data.
- **OpenCV**: For image processing tasks.


## Installation

To run the Smart Pokédex locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/smart-pokedex.git
   cd smart-pokedex

2. **Install Dependencies**:
Make sure you have Python 3.7+ installed. Then, install the required libraries of requirements.txt using pip:

    ```bash
    pip install -r requirements.txt

3. **Download Dataset**:
Download the Pokémon image dataset from Kaggle or any other source.
Place the dataset in the appropriate directory

4. **Set Up the Database**:
Run the create_db_table.py script to create and populate the SQLite database:
    ```bash
    python create_db_table.py
    
5. **Train the Model (Optional)**:
If you want to retrain the CNN model, run the model_training.py script:
    ```bash
    python model_training.py

6. **Run the Application**:
Start the Streamlit app by running:

    ```bash
    streamlit run Pokedex.py

## Usage
- **Launch the Application**:
After running the Streamlit app, open the provided URL in your browser to access the Pokédex.

- **View Pokémon Information**:
Browse through the database to view detailed information about all Pokémon.

- **Classify Pokémon Images**:
Use the interface to upload an image of a Pokémon. The app will classify the image only if it belongs to one of the first 151 Pokémon. If the Pokémon is not in the first generation, the classifier will not recognize it.


## Limitations
- **Image Classifier**: The image classifier is trained only on the first 151 Pokémon (Generation 1). It will not recognize Pokémon from other generations.
- **Dataset**: Ensure the training and testing datasets are correctly placed in the PokemonData_train and PokemonData_test directories.


## Future Improvements
- Expand the image classifier to include Pokémon from other generations.
- Add more advanced features, such as battle simulations or team-building tools.
- Improve the UI/UX with additional interactive elements.




