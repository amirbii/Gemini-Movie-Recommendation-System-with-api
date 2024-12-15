import gradio as gr
import google.generativeai as genai

genai.configure(api_key="AIzaSyC4MnvV5ebUP1QRey4OTkWc2wZOVVJVwbE1")
model = genai.GenerativeModel('gemini-pro')


def suggest_Movie(watched_Movie):
    chat = model.start_chat(history=[
        {"role": "user", "parts": ["You are a movie recommendation system. Based on user input, suggest 10 movies."]},
    ])
    try:
        response = chat.send_message(watched_Movie)
        return response.text
    except Exception as e:
        return f"An error occurred: {e}"


iface = gr.Interface(
    fn=suggest_Movie,
    inputs=gr.Textbox(label="Enter a movie you liked:"),
    outputs=gr.Textbox(label="Movie Recommendations"),
    title="Gemini Movie Recommendation System",
    description="Enter a movie you liked and I'll suggest 10 similar movies."
)

iface.launch()
