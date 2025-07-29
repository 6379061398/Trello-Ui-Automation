# Trello Board Automation using Playwright + TypeScript
This project automates a series of actions on a Trello board using Playwright with TypeScript. It performs login, board creation, list and card setup, card dragging between lists, label and description management, and file attachment.

# Features
✅ Login to Trello using secure credentials from .env
✅ Create a new board with timestamped name
✅ Create three lists: To Do, In Progress, Done
✅ Add a card to each list
✅ Add labels and descriptions to cards
✅ Drag and drop a card from "To Do" → "In Progress" → "Done"
✅ Attach a PDF file to the card
✅ Final assertion to ensure the card exists in the "Done" list

# Setup Instructions
1. Clone the Repository
  git clone https://github.com/yourusername/trello-playwright-automation.git
  cd trello-playwright-automation

2. Install Dependencies
   npm install

3. package.json
   {
  "name": "trello-playwright-automation",
  "version": "1.0.0",
  "scripts": {
    "test": "npx playwright test"
  },
  "dependencies": {
    "dotenv": "^16.0.0"
  },
  "devDependencies": {
    "@playwright/test": "^1.44.0",
    "typescript": "^5.0.0"
  }
}

4. Add .env File
   TRELLO_EMAIL=your-email@example.com
   TRELLO_PASSWORD=your-trello-password

5. Add Attachment File
   Place your resume or PDF file (e.g. SAMARJEET_Resume.pdf) inside the project directory.

6. Run the Test
   npx playwright test

# Folder Structure
trello-playwright-automation/
│
├── e2e/
│   └── assignment.spec.ts      # Main test script
├── .env                        # Environment variables
├── SAMARJEET_Resume.pdf        # Attachment file (example)
├── package.json
├── tsconfig.json
├── playwright.config.ts
└── README.md                   # This file

