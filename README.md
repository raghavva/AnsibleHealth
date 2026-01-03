## Markdown ➜ Google Doc (Colab)

Convert the provided meeting-notes markdown into a well-formatted Google Doc using the Google Docs API, with headings, nested bullets, checkboxes, mention styling, and footer formatting.

### What’s inside
- `assessment.ipynb`: Colab-ready notebook that authenticates with Google, parses the markdown, and builds the Doc via `documents.batchUpdate`.
- `process.md`: Source markdown meeting notes.

### Quick start (Colab)
1) Upload both `assessment.ipynb` and `process.md` to Google Colab (or open from Drive/GitHub once you create a repo).  
2) Run the notebook cells top-to-bottom. The `%pip install` cell refreshes the Google API client libraries.  
3) When prompted, complete the OAuth flow. (Google Docs API must be enabled for your account/project.)  
4) A new Doc link prints at the end; open it to see the formatted output.

### Requirements
- Google account with Google Docs API enabled.
- Colab runtime with internet access.
- OAuth client: Colab’s built-in flow works by default. If you prefer your own OAuth client, upload `client_secret.json` before running the auth cell.


### Suggested repo steps
- Create a new public GitHub repo, add `assessment.ipynb`, `process.md`, and this `README.md`, then push. Example:  
  ```bash
  git init
  git add assessment.ipynb process.md README.md
  git commit -m "Add Colab notebook for markdown to Google Doc"
  git branch -M main
  git remote add origin <your-repo-url>
  git push -u origin main
  ```


