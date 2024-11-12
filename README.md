# ECE590 Final Project

This repository contains our ECE590 final project paper, written in LaTeX using the IEEE template.

## Initial Setup

### 1. Installing LaTeX and TeXstudio

#### Windows
1. Download and install MiKTeX from [https://miktex.org/download](https://miktex.org/download)
2. Download and install TeXstudio from [https://www.texstudio.org](https://www.texstudio.org)

#### macOS
1. Download and install MacTeX from [https://www.tug.org/mactex/](https://www.tug.org/mactex/)
2. Download and install TeXstudio from [https://www.texstudio.org](https://www.texstudio.org)

#### Linux
```bash
# For Ubuntu/Debian
sudo apt-get update
sudo apt-get install texlive-full texstudio

# For Fedora
sudo dnf install texlive-scheme-full texstudio
```

### 2. Testing Your LaTeX Installation

1. Open TeXstudio
2. First, open and compile the IEEE template file (`IEEE template.tex`)
   - This file contains important formatting instructions and examples
   - Keep this file as a reference for LaTeX commands and styling
   - A successful compilation confirms your LaTeX setup is working
3. Then, open the paper file (`paper.tex`)
   - This is where we'll write our actual project paper
   - It's based on the IEEE template but stripped down to essentials
4. Click the "Build & View" button (green play button) or press F5 to compile

## GitHub Setup and Workflow

### First Time Git Setup

1. Install Git on your computer:
   - Windows: Download from [https://git-scm.com/download/windows](https://git-scm.com/download/windows)
   - Mac: Open Terminal and type `git --version`. Follow the prompts to install.
   - Linux: `sudo apt-get install git` (Ubuntu/Debian) or `sudo dnf install git` (Fedora)

2. Configure Git (replace with your details):
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Initial Repository Setup (Do This Once)

1. Create a directory for your project:
```bash
# On Windows:
mkdir C:\Projects\ECE590
cd C:\Projects\ECE590

# On Mac/Linux:
mkdir ~/Projects/ECE590
cd ~/Projects/ECE590
```

2. Clone the repository:
```bash
git clone https://github.com/Brent-Dickinson/ECE590.git .
```
Note: The period (.) at the end tells Git to clone into the current directory

### Daily Workflow

#### Starting Your Work Session:
1. Open your terminal/command prompt
2. Navigate to your project directory:
```bash
# On Windows:
cd C:\Projects\ECE590

# On Mac/Linux:
cd ~/Projects/ECE590
```

3. Get the latest changes:
```bash
git pull origin main
```

#### While Working:
1. After making changes (like editing paper.tex), check what files you've modified:
```bash
git status
```

2. Add your changes:
```bash
# To add all changes:
git add .

# Or to add specific files:
git add paper.tex
git add figures/new-figure.png
```

3. Save (commit) your changes:
```bash
git commit -m "Write a message describing what you changed"
```
Example messages:
- "Added introduction section"
- "Updated methodology"
- "Added new figure for results"

#### Ending Your Work Session:
1. Push your changes to GitHub:
```bash
git push origin main
```

### If Something Goes Wrong

1. If you made mistakes and want to start over:
```bash
git fetch origin
git reset --hard origin/main
```
WARNING: This will delete all your local changes!

2. If push is rejected:
```bash
# Get latest changes first
git pull origin main

# Then try pushing again
git push origin main
```

3. If you see "merge conflicts":
   - Contact your partner before proceeding
   - Decide whose changes to keep
   - Or seek help if unsure

## Repository Structure

```
├── IEEE template.tex  # Original IEEE template with formatting instructions
├── paper.tex         # Our project paper
└── figures/          # Directory for images and figures
```

## Bibliography Notes

The bibliography will be written directly in the paper.tex file using the IEEE format:

```latex
\begin{thebibliography}{00}
\bibitem{ref1} Author(s), "Title of paper," Journal Name, vol. x, no. x, pp. xxx-xxx, Month Year.
\bibitem{ref2} Author(s), "Title of book," Publisher, Year.
\end{thebibliography}
```

To cite references in the text, use the `\cite{ref1}` command.

## Additional Resources

- [LaTeX Tutorial](https://www.latex-tutorial.com)
- [IEEE Template Documentation](https://www.ieee.org/conferences/publishing/templates.html)
- [Git Documentation](https://git-scm.com/doc)
