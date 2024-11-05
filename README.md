# Shruk.com




# Shruk Website GitHub Repository Setup

## Repository Structure
```
shruk-website/
├── index.html
├── README.md
└── shruks/
    ├── shruk1.txt
    ├── shruk2.txt
    ├── shruk3.txt
    └── ...
```

## Shruk File Format
Each shruk file (e.g., `shruk1.txt`) should follow this format:
```
[Kashmiri Text Here]
[English Translation Here]
[French Translation Here]
[German Translation Here]
[Russian Translation Here]
```

Example `shruk1.txt`:
```
پوشہِ متٮ۪ن یِمن ابدالن خۄش کٔلمَن بوٗزِکھ معنے گوش روٚٹُکھ پٮ۪ٹھ سنگاسن یِمن لعلن مۄل کُس زانے
Those beautiful virtuous souls Sought the meanings of the verses divine! They found their place on the thrones. Who can know their proper worth.
Ces belles ȃmes vertueuses Cherchaient le sens des vers divins! Ils trouverent leur place sur les trȏnes. Qui peut connaitre leur juste valeur?
Diese schönen tugendhaften Seelen Suchten nach der Bedeutung der göttlichen Verse! Sie fanden ihren Platz auf den Thronen. Wer kann ihren wahren Wert kennen?
Эти прекрасные добродетельные души Искали смысл божественных стихов! Нашли своё место на престолах. Кто может знать их цену?
```

## Setup Instructions

1. Create a new GitHub repository
   - Go to GitHub and create a new repository named "shruk-website"
   - Initialize it with a README.md

2. Configure the repository
   - Clone the repository to your local machine
   - Create a `shruks` folder
   - Add the `index.html` file (provided above) to the root directory

3. Update the configuration
   In the `index.html` file, update the config object with your GitHub details:
   ```javascript
   const config = {
       owner: 'YOUR_GITHUB_USERNAME',
       repo: 'shruk-website',
       branch: 'main',
       baseUrl: 'https://api.github.com/repos'
   };
   ```

4. Add Shruks
   - Create individual text files for each Shruk in the `shruks` folder
   - Name them as `shruk1.txt`, `shruk2.txt`, etc.
   - Follow the file format shown above

5. Deploy the website
   - Enable GitHub Pages in your repository settings
   - Set the source to the main branch
   - Your website will be available at `https://[your-username].github.io/shruk-website`

## Managing Shruks

### To add a new Shruk:
1. Create a new file in the `shruks` folder named `shrukX.txt` (where X is the number)
2. Add the content following the format above
3. Commit and push to GitHub

### To modify a Shruk:
1. Edit the corresponding text file
2. Commit and push the changes

### To remove a Shruk:
1. Delete the corresponding text file
2. Commit and push the changes

## Important Notes
- Make sure to maintain proper formatting in the text files
- Each translation should be on a new line
- The website will automatically load Shruks from numbers 1 to 99
- All text files should use UTF-8 encoding to properly display Kashmiri text
