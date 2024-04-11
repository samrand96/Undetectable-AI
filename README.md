# Undetectable-AI
Welcome to the Undetectable AI Tool! This script is designed to huminize ChatGPT and other text-based content. It offers efficient DOCX file manipulation, including text translation, humanization, grammar correction, and content evaluation. Powered by leading Python libraries and external services, it provides a seamless solution for automating document workflows. With customizable options via command-line arguments, it's perfect for professionals and enthusiasts looking to streamline text processing tasks.

## Usage

To use the Python DOCX Processor, follow these steps:

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/samrandhaji/Undetectable-AI
    ```

2. Navigate to the repository directory:

    ```bash
    cd Undetectable-AI
    ```

3. Install the required dependencies using pip:

    ```bash
    pip install -r requirements.txt
    ```

4. Run the script with the desired options:

    ```bash
    python docx_processor.py <file_path> [--output_file_path <output_file_path>] [--model <model_name>] [--target_lang <target_language>] [--grammar] [--chatgpt]
    ```

    - `<file_path>`: Path to the original DOCX file.
    - `--output_file_path`: (Optional) Path to save the processed DOCX file. If not provided, a timestamped filename will be generated.
    - `--model`: (Optional) Model name for ollama. Default is "dolphin-mistral:latest".
    - `--target_lang`: (Optional) Language code for intermediate translation. Default is "arabic".
    - `--grammar`: (Optional) Enable grammar correction. Off by default.
    - `--chatgpt`: (Optional) Use ChatGPT instead of regular humanization. Off by default.

5. The processed document will be saved as specified or with a timestamped filename in the current directory.

Example:

```bash
python docx_processor.py input.docx --output_file_path processed.docx --model dolphin-mistral:latest --target_lang russian --grammar --chatgpt
