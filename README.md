# DocuBrain - Your Smart PDF Assistant

## What is DocuBrain?

DocuBrain is a smart chatbot that answers questions **only** based on information in your PDF files. Think of it as having a personal assistant who has read all your documents and can answer questions about them instantly.

### Why is this useful?

- **Accurate & Trustworthy**: The chatbot only answers based on what's in your PDFs. It won't make up answers using general knowledge.
- **Perfect for Healthcare, Legal, and Business**: When accuracy is critical, DocuBrain ensures all answers come directly from your documents.
- **Conversational**: Ask follow-up questions naturally. The chatbot remembers your conversation history.
- **Fast & Efficient**: Uses AI to understand what you're asking and finds relevant information quickly.

---

## Getting Started

### What You'll Need

1. **Python 3.8 or higher** - Download from [python.org](https://www.python.org/)
2. **OpenAI API Key** - Get a free one from [OpenAI](https://platform.openai.com/api-keys) (requires a paid account)
3. **Your PDF Files** - The documents you want to ask questions about

### Step-by-Step Setup

#### 1. **Create a Project Folder**
Open your terminal/command prompt and create a project folder.

#### 2. **How to Use DocuBrain**

### Running the App

1. Open the Jupyter notebook `docuBrain.ipynb` in VS Code or your preferred Jupyter environment
2. Run the cells in sequence from top to bottom:
   - Cell 1: Install dependencies
   - Cell 2: Import required libraries
   - Cell 3: Load environment variables and API key
   - Cells 4-8: Define helper functions
   - Cell 9: Define main function
   - Cell 10: Execute the main application

3. When prompted, enter your PDF file paths (comma-separated)

### Example Conversation

```
DocuBrain - Upgraded Edition (PyMuPDF, async, batching)
Enter PDF file paths (comma separated): C:\path\to\machinelearning.pdf

Embedding 353 chunks in batches...
PDF(s) processed. You can now ask questions. Type 'exit' to quit.

Your question: What is machine learning?
Bot: Machine learning is a subfield of computer science that involves building 
algorithms that rely on examples of a phenomenon to solve practical problems...

Your question: What is a calculator?
I don't know.
(Because 'calculator' is not mentioned in the PDF)

Your question: exit
Goodbye!
```

### Tips for Best Results

1. **Use Full File Paths**: When entering PDF paths, use the complete path:
   - Windows: `C:\Users\YourName\Documents\report.pdf`
   - Mac/Linux: `/Users/YourName/Documents/report.pdf`

2. **Multiple PDFs**: You can ask about multiple PDFs at once by separating paths with commas:
   ```
   Enter PDF file paths: C:\docs\file1.pdf, C:\docs\file2.pdf, C:\docs\file3.pdf
   ```

3. **Ask Natural Questions**: DocuBrain understands natural language, so you can ask:
   - "What is machine learning?"
   - "Tell me about machine learning"
   - "How does machine learning work?"
   - "What are the types of learning?"

4. **Type 'exit'**: To quit the conversation, simply type `exit` and press Enter.

---

## Important Features

### ✅ **Only Uses Your PDFs**
DocuBrain will **only** answer questions based on information in your PDFs. If something isn't in your documents, it will honestly say "I don't know" instead of guessing or making something up.

**Example:**
- If your PDF doesn't mention "calculators," and you ask "What is a calculator?", it will say "I don't know" (even though it knows what a calculator is generally).

### ✅ **Remembers Your Conversation**
The chatbot keeps track of your chat history, so you can ask follow-up questions naturally.

### ✅ **Fast Processing**
Even with large PDFs (hundreds of pages), the bot processes them quickly using smart embedding technology.

---

## Troubleshooting

### Problem: "No valid PDFs found"
**Solution**: Check that:
- The file path is spelled correctly
- The file exists and is a PDF
- You're using the full path (not just the filename)

### Problem: "I don't know" to all questions
**Solution**: This might mean:
- The PDF doesn't contain information about your question
- The question is phrased very differently from the PDF text
- Try rephrasing your question more naturally

### Problem: "Error: Invalid OpenAI API Key"
**Solution**:
- Check that your API key is pasted correctly as `Jupyter Environment Variables`.
- Make sure there are no extra spaces before or after the key
- Verify your OpenAI account has credits/is active

### Problem: "ModuleNotFoundError"
**Solution**: Run the installation cell again.
---

## Files Explained

- **docuBrain.ipynb** - The main Jupyter notebook application (run this)
- **requirements.txt** - List of software packages needed
- **.env** - Your OpenAI API key (keep this private!)
- **README.md** - This file

---

## Privacy & Security

- Your PDFs are **not** sent to OpenAI
- Only the questions and retrieved text are sent to OpenAI for answer generation
- Your OpenAI API key is kept private as the `Jupyter Environment` variable (don't share it!)

---

## What Makes DocuBrain Different?

Unlike regular ChatGPT:
- ✅ Uses your specific documents (not general internet knowledge)
- ✅ Perfect for private/sensitive information
- ✅ Gives "I don't know" instead of making up answers
- ✅ Ideal for healthcare, legal, and business use cases

---

## Need Help?

If something isn't working:
1. Make sure all installation steps are complete
2. Check that your OpenAI API key is valid
3. Ensure your PDFs are in the correct location
4. Try with a simpler PDF first to test

---

**Enjoy your smart PDF assistant! 🎉**
