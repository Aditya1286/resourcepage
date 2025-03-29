# 📚 Library Resource Hub

A modern, responsive web application that allows students to browse, search, and download educational resources from your institution's library. Built with HTML, Tailwind CSS, and vanilla JavaScript.

![Library Resource Hub Screenshot](/api/placeholder/800/400)

## 🌟 Features

- **Intuitive Resource Browsing**: Categorized view of all available educational materials
- **Advanced Search Functionality**: Find resources by title, author, subject, or type
- **Responsive Design**: Works seamlessly on desktops, tablets, and mobile devices
- **Download Management**: Track download history and resume interrupted downloads
- **Resource Collections**: Save favorites and create custom resource collections
- **Dark/Light Mode**: Toggle between visual themes for comfortable viewing
- **Accessibility Focused**: Built with WCAG guidelines in mind for all students

## 🛠️ Technology Stack

- **HTML5**: Semantic markup for better structure and accessibility
- **Tailwind CSS**: Utility-first CSS framework for responsive design
- **JavaScript**: Vanilla JS for interactivity and functionality
- **LocalStorage API**: For saving user preferences and download history
- **Fetch API**: For retrieving resource data

## 📋 Requirements

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection for initial load and resource downloads

## 🚀 Getting Started

### For Students

1. Visit the Library Resource Hub at your institution's URL
2. Log in with your student credentials
3. Browse resources by category or use the search function
4. Click on any resource to view details
5. Use the download button to save resources to your device

### For Developers

1. Clone the repository
```bash
git clone https://github.com/yourinstitution/library-resource-hub.git
cd library-resource-hub
```

2. Open the project in your code editor

3. Install dependencies (if you plan to modify Tailwind)
```bash
npm install
```

4. For development with Tailwind CSS
```bash
npm run dev
```

5. Build for production
```bash
npm run build
```

## 📁 Project Structure

```
library-resource-hub/
├── index.html              # Main entry point
├── css/
│   └── styles.css          # Compiled Tailwind CSS
├── js/
│   ├── main.js             # Main application logic
│   ├── search.js           # Search functionality
│   ├── downloads.js        # Download management
│   └── collections.js      # User collections logic
├── assets/
│   ├── icons/              # UI icons
│   └── images/             # Static images
├── data/
│   └── resources.json      # Sample resource data
├── tailwind.config.js      # Tailwind configuration
└── package.json            # Project dependencies
```

## 🔧 Customization

### Adding New Resources

Resources are managed through the `resources.json` file. The format for each resource is:

```json
{
  "id": "unique-id",
  "title": "Resource Title",
  "author": "Author Name",
  "description": "Brief description of the resource",
  "type": "pdf",
  "subject": "Mathematics",
  "category": "Textbooks",
  "downloadUrl": "path/to/resource.pdf",
  "coverImage": "path/to/cover.jpg",
  "dateAdded": "2025-03-15",
  "size": "12.4MB",
  "tags": ["calculus", "undergraduate", "recommended"]
}
```

### Modifying Categories

To add or modify resource categories, edit the `categories` array in `main.js`:

```javascript
const categories = [
  { id: "textbooks", name: "Textbooks", icon: "book" },
  { id: "journals", name: "Academic Journals", icon: "journal" },
  // Add more categories here
];
```

## 🔍 Search Functionality

The search system supports:

- Full-text search across all resource fields
- Filtering by category, type, and subject
- Sorting by relevance, date added, or popularity
- Advanced search operators (AND, OR, NOT)

Example search query:
```
physics AND (quantum OR relativity) NOT beginner
```

## 🌐 Browser Support

- Chrome (last 2 versions)
- Firefox (last 2 versions)
- Safari (last 2 versions)
- Edge (last 2 versions)

## 🔒 Privacy and Security

- No student data is sent to external servers
- Download history is stored locally in the browser
- Authentication is handled through your institution's SSO system

## 🤝 Contributing

If you'd like to contribute to this project:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- [Heroicons](https://heroicons.com/) for the beautiful SVG icons
- [Academic Resource Database](https://example.org) for the sample resource data

## 📞 Support

For support, please contact the library IT department:
- Email: library-it@yourinstitution.edu
- Help Desk: Building A, Room 101
- Hours: Monday-Friday, 9am-5pm

---

Designed and maintained by the Library Technology Team at [Your Institution Name]
