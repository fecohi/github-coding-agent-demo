# 🏀 NBA Player Directory

A modern, interactive web application built with Streamlit for exploring NBA player data. Browse through hundreds of players with advanced filtering, sorting, and search capabilities.

![NBA Player Directory Screenshot](https://github.com/user-attachments/assets/116ac70c-d1c3-4d83-977f-1977d58a8432)

## ✨ Features

### 🔍 Advanced Search & Filtering
- **Text Search**: Search across player names, positions, schools, and countries
- **Position Filter**: Multi-select dropdown for specific positions (Guard, Forward, Center, etc.)
- **Country Filter**: Filter players by their country of origin
- **Draft Year Range**: Interactive slider to filter by draft year (2003-2022)
- **Height Filter**: Range slider to filter players by height in inches (69"-88", equivalent to 5'9" - 7'4")
- **Weight Filter**: Range slider to filter players by weight in pounds (160-290 lbs)

### 📊 Data Visualization
- **Card Layout**: Beautiful player cards with photos and detailed information
- **Responsive Grid**: Clean 3-column layout that adapts to your screen
- **Player Images**: Individual player photos with fallback placeholders
- **Comprehensive Stats**: Position, height, weight, age, country, school, and draft information

### ⚙️ Customization Options
- **Flexible Sorting**: Sort by name, position, country, draft year, height, weight, or age
- **Pagination Controls**: Adjustable page sizes (6, 9, 12, 24, or 48 players per page)
- **Raw Data View**: Expandable table view for detailed data analysis
- **Real-time Updates**: Instant filtering and search results

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Geronimo-Basso/github-coding-agent-demo.git
   cd github-coding-agent-demo
   ```

2. **Create and activate virtual environment**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   The app will automatically open at `http://localhost:8501`

## 📁 Project Structure

```
github-coding-agent-demo/
├── app.py                    # Main Streamlit application
├── requirements.txt          # Python dependencies
├── README.md                # This file
└── nba-mock-data/           # Data directory
    ├── players.csv          # Player dataset (548 players)
    └── img/                 # Player images directory
        ├── 1630173.png      # Individual player photos
        ├── 203500.png
        └── ...
```

## 📊 Data Schema

The application uses a CSV dataset with the following fields:

| Field | Description | Example |
|-------|-------------|---------|
| `playerid` | Unique player identifier | `1630173` |
| `fname` | First name | `Precious` |
| `lname` | Last name | `Achiuwa` |
| `position` | Playing position | `Forward` |
| `height` | Player height | `6-8` |
| `weight` | Player weight (lbs) | `225` |
| `birthday` | Birth date | `1999-09-19` |
| `country` | Country of origin | `Nigeria` |
| `school` | College/University | `Memphis` |
| `draft_year` | NBA draft year | `2020` |
| `draft_round` | Draft round | `1` |
| `draft_number` | Draft pick number | `20` |

## 🛠️ Technical Details

### Dependencies
- **Streamlit** `>=1.38.0` - Web app framework
- **Pandas** `>=2.2.0` - Data manipulation and analysis
- **Python** `>=3.8` - Programming language

### Key Features Implementation
- **Caching**: Uses `@st.cache_data` decorator for optimal performance
- **Error Handling**: Graceful fallbacks for missing images and data
- **Responsive Design**: Mobile-friendly layout with flexible columns
- **Data Validation**: Automatic data cleaning and normalization

## 🎯 Usage Examples

### Search for Specific Players
- Type "LeBron" in the search box to find LeBron James
- Search "Duke" to find all players from Duke University
- Search "Canada" to find all Canadian players

### Filter by Multiple Criteria
1. Select "Guard" from the Position filter
2. Choose "USA" from the Country filter  
3. Adjust the Draft Year slider to 2015-2020
4. Set Height range to 72-78 inches (6'0" - 6'6")
5. Set Weight range to 190-220 lbs
6. Sort by "height" to see the tallest guards within the selected range

### Browse and Explore
- Use pagination to browse through all 548 players
- Click the "Raw table" expander to see the complete dataset
- Experiment with different sort orders to discover patterns

## 🔄 Future Enhancements

- [ ] **Team Filtering**: Add NBA team-based filters
- [ ] **Advanced Statistics**: Include performance metrics and career stats
- [ ] **Data Export**: Download filtered datasets as CSV
- [ ] **Comparison Tool**: Side-by-side player comparisons
- [ ] **Data Caching**: Implement advanced caching strategies
- [ ] **API Integration**: Real-time NBA data updates
- [ ] **Unit Tests**: Comprehensive test coverage for data utilities

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙋‍♂️ Support

If you have any questions or run into issues:
- Check the [Issues](https://github.com/Geronimo-Basso/github-coding-agent-demo/issues) page
- Create a new issue with detailed information about your problem
- Include your Python version and operating system

---

<div align="center">
  <p><strong>Built with ❤️ using Streamlit and Python</strong></p>
  <p><em>Generated with help from GitHub Copilot Coding Agent</em></p>
</div>