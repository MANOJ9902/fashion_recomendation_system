# Fashion-recommender-system
A Deep Learning based Fashion Recommender System using the ResNET50


Streamlit web application for a Fashion Recommender System and T-shirt Designer. Here is a breakdown of the key components and functionalities of the code:
1.	Importing Libraries:
	The code starts by importing various Python libraries, including Streamlit for building the web app, PIL (Pillow) for image manipulation, NumPy, TensorFlow for deep learning tasks, Scikit-learn for nearest neighbor recommendation, and other necessary modules.
2.	Streamlit App Initialization:
	It initializes a Streamlit app with the title "Fashion Recommender System and T-shirt Designer."
3.	Upload T-shirt Image:
	Users can upload a T-shirt image (JPEG or PNG with a transparent background). The uploaded image is displayed on the web app.
4.	Customization Options:
	Users can customize the T-shirt by uploading a logo with a transparent background, adjusting the logo size, and specifying the vertical position. When customization options are applied, the logo is added to the T-shirt, and the customized T-shirt is displayed.
5.	Generate Clothes with DALL-E:
	Users can input a prompt, select an image size, and generate clothes using the OpenAI DALL-E API. The generated clothes image is displayed on the web app.
6.	Recommendation Section:
	This section focuses on recommending outfits based on user preferences.
7.	Feature Extraction and Recommendation:
	Precomputed features and filenames are loaded from 'embeddings.pkl' and 'filenames.pkl.'
	The ResNet-50 model is loaded for feature extraction. Features are extracted from uploaded images using this model.
	A recommendation function is provided that finds similar images based on extracted features.
8.	User Interaction for Recommendations:
	Users can upload an image, specify the number of recommendations they want (between 1 and 50), and see recommended outfits based on their uploaded image.
9.	File Saving and Error Handling:
	There are functions to save uploaded files and handle potential errors during file upload.
10.	OpenAI Integration:
	The code utilizes the OpenAI DALL-E API to generate clothes images based on user prompts.
11.	Streamlit Web App Interface:
	The Streamlit app interface includes sidebars for customization options, generating clothes, and displaying recommendations.
12.	Displaying Images:
	Images (T-shirt, customized T-shirt, generated clothes, and recommended outfits) are displayed within the app using Streamlit's image display functionality.
Overall, this code combines image customization, AI-based image generation, and outfit recommendations in a single web application, making it a versatile tool for fashion enthusiasts. Users can upload T-shirt designs, customize them with logos, generate unique clothing items, and receive outfit recommendations based on their preferences.

