# Amazon OA Prep 🚀

A clean, minimalistic React web application designed to help you prepare for Amazon Online Assessment (OA) coding interviews. This website provides a curated collection of coding problems with detailed algorithms, step-by-step solutions, and code examples.

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Search Functionality**: Filter problems by title, topic, or difficulty level
- **Detailed Solutions**: Each problem includes:
  - Algorithm explanation with approach
  - Step-by-step solution breakdown
  - Time and space complexity analysis
  - Complete code implementation
  - Example test cases with explanations
- **Clean UI**: Minimalistic design focused on readability and learning
- **No Backend Required**: All data is stored in JSON format for quick loading

## Tech Stack

- **React 18** - Modern React with hooks
- **Vite** - Fast build tool and development server
- **CSS3** - Custom responsive styling with CSS variables
- **JSON** - Simple data storage without database complexity

## Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd amazon-oa-prep
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser and visit `http://localhost:5173`

### Build for Production

```bash
npm run build
```

The built files will be in the `dist` directory, ready for deployment.

## Project Structure

```
src/
├── components/           # React components
│   ├── SearchBar.jsx    # Search functionality
│   ├── ProblemList.jsx  # List of problems
│   ├── ProblemCard.jsx  # Individual problem display
│   └── *.css           # Component styles
├── data/
│   └── problems.json    # Problem data storage
├── App.jsx             # Main application component
├── App.css            # Global styles
├── main.jsx           # React entry point
└── index.css          # Base styles
```

## Adding New Problems

To add new problems, edit `src/data/problems.json` following this structure:

```json
{
  "id": 6,
  "title": "Problem Title",
  "difficulty": "Easy|Medium|Hard",
  "topic": "Array, Hash Table, etc.",
  "description": "Problem description...",
  "algorithm": {
    "approach": "Algorithm name",
    "steps": ["Step 1", "Step 2", "..."],
    "timeComplexity": "O(n)",
    "spaceComplexity": "O(1)"
  },
  "code": {
    "language": "javascript",
    "solution": "function solution() { ... }"
  },
  "examples": [
    {
      "input": "Input example",
      "output": "Expected output",
      "explanation": "Why this works"
    }
  ]
}
```

## Sample Problems Included

The website comes with 5 sample problems covering different difficulty levels:

1. **Two Sum** (Easy) - Hash Table approach
2. **Amazon Fresh Promotion** (Medium) - Two Pointers technique
3. **Critical Connections** (Hard) - Graph algorithms with DFS
4. **Package Delivery** (Medium) - Greedy algorithms
5. **Minimum Window Substring** (Hard) - Sliding Window technique

## Customization

### Styling
- Edit CSS variables in `src/App.css` to change the color scheme
- Modify component styles in individual CSS files
- The design uses a mobile-first responsive approach

### Adding Features
- Search filters can be extended in `ProblemList.jsx`
- New problem properties can be added to the JSON structure
- Additional tabs can be added to `ProblemCard.jsx`

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Inspired by the need for better Amazon OA preparation resources
- Built with modern web technologies for optimal performance
- Designed with accessibility and user experience in mind

---

**Happy Coding! 💻✨**

*Remember: Consistent practice is the key to acing your Amazon OA!*