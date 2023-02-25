# Encrypto
This is a Python Flask web application that allows users to encrypt and decrypt files using Fernet encryption from the cryptography library. The app has two main routes: /encrypt and /decrypt.

The /encrypt route allows users to upload a file, encrypt it using a randomly generated key, and then download the encrypted file along with the key as a zip file. The app first checks if the file is valid and saves it to the server's uploads folder. It then generates a random key and uses it to encrypt the uploaded file. The encrypted file and key are then zipped and sent to the user for download.

The /decrypt route allows users to upload an encrypted file and its corresponding key, decrypt the file, and then download the decrypted file. The app first checks if both files are valid and saves them to the server's uploads folder. It then loads the key from the key file and uses it to decrypt the uploaded file. The decrypted file is then saved to the server's downloads folder and sent to the user for download.

The app also includes a /clear route that allows users to clear the server's uploads and downloads folders.




## Getting Started
### Prerequisites
To run this app, you will need:

* Python 3.x
* Flask
##Installation
Clone this repository:
```
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

### Create a virtual environment:

```
python3 -m venv venv
source venv/bin/activate  # on Windows, use venv\Scripts\activate.bat
```

### Install the required packages:

```
pip install -r requirements.txt
```
### Usage
Start the Flask app:

```
flask run
```

Open your web browser and go to http://localhost:5000.


## Styling with Tailwind CSS
This app uses Tailwind CSS for styling. To customize the styles, edit the styles.css file in the static folder. You can use the Tailwind CSS classes to style your HTML elements.

For more information, see the [Tailwind CSS documentation](https://tailwindcss.com/docs).

### License
This project is licensed under the MIT License - see the LICENSE file for details.
