# YouTube Video Chaptering Using Python

This project provides a comprehensive tool for analyzing YouTube video transcripts. The script allows users to extract transcripts from YouTube videos, save them in a CSV file, and perform various text analyses including word frequency, topic modeling, and chapter segmentation. 

## Features

- **Extract YouTube Video Transcripts**: Automatically fetches transcripts from a YouTube video given its URL.
- **Save Transcripts to CSV**: Saves the video title and transcript text into a CSV file.
- **Text Analysis**:
  - **Text Length Distribution**: Visualizes the distribution of text lengths in the transcript.
  - **Common Word Analysis**: Identifies and visualizes the most frequent words in the transcript.
  - **Topic Modeling**: Uses Non-Negative Matrix Factorization (NMF) to identify and display topics present in the transcript.
- **Chapter Segmentation**: Analyzes the logical breaks in the transcript to create readable chapters, each associated with a dominant topic.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/KishoreRaghupathy/Video-Chaptering-Using-Python/
    cd youtube-transcript-analyzer
    ```

2. Install the required Python packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Set up your Google API key:
    - Go to the [Google Developers Console](https://console.developers.google.com/).
    - Create a project and enable the YouTube Data API v3.
    - Generate an API key and replace the placeholder `API_KEY` in the script with your key.

## Usage

1. **Running the Script**: 
    ```bash
    python transcript_analyzer.py
    ```
   You will be prompted to enter a YouTube video URL. The script will then process the video, fetch the transcript, save it to a CSV file, and perform various analyses.

2. **Analyzing the Transcripts**:
    - After running the script, the CSV file containing the transcript will be generated in the same directory.
    - The script also provides visualizations and outputs directly to the console, including word frequency analysis, topic modeling, and chapter segmentation.

## Example Output

- **Text Length Distribution**: A histogram displaying the distribution of text segment lengths in the transcript.
- **Common Words**: A bar chart showing the top 20 most frequent words in the transcript.
- **Identified Topics**: A list of topics extracted from the transcript using NMF.
- **Final Chapter Points with Names**: A list of chapters with their respective start times and names based on key phrases.

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- scikit-learn
- google-api-python-client
- youtube-transcript-api

Install dependencies using:
```bash
pip install pandas numpy matplotlib scikit-learn google-api-python-client youtube-transcript-api
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue.

