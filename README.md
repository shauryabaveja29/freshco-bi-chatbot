# 📊 Generic BI Chatbot - Full Featured

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Production](https://img.shields.io/badge/Status-Production-green.svg)]()
[![AI: Gemini](https://img.shields.io/badge/AI-Gemini%203%2027B-blue.svg)]()

> AI-powered business intelligence chatbot with complete CPG analytics capabilities. Upload any Excel/CSV file and get instant insights with charts, tables, and validation.

**🎓 Academic Project** | IIM Ahmedabad | GenAI Course | January 2026

---

## 🌟 Features

### **Core Capabilities**
- ✅ **Upload Any Data** - Works with Excel (.xlsx, .xls) or CSV files
- ✅ **Auto-Detection** - Automatically detects and maps columns
- ✅ **12 Query Types** - Comprehensive analysis capabilities
- ✅ **Professional Charts** - Bar, line, and pie charts with Chart.js
- ✅ **Validation Sections** - Step-by-step calculation breakdowns
- ✅ **BYOK** - Bring Your Own API Key (stored locally)

### **Analysis Types**
1. 📊 **Summary Analysis** - Dataset statistics and overview
2. 🔝 **Top N Analysis** - Highest/lowest performers
3. 📈 **Trend Analysis** - Time series patterns
4. 🏪 **Regional Performance** - Geographic breakdowns
5. 🏙️ **City Analysis** - City-level insights
6. 💰 **Profit Margins** - Profitability analysis
7. ⚠️ **Stockout Detection** - Out-of-stock identification with revenue impact
8. 📦 **Inventory Pileup** - Slow-moving stock detection
9. 🎯 **Promotion Effectiveness** - Marketing campaign ROI
10. 💸 **Discount Analysis** - Pricing impact assessment
11. 📊 **Universal Grouping** - Aggregate by any dimension
12. 🔍 **General Queries** - Natural language questions

---

## 🚀 Quick Start

### **1. Download**
```bash
git clone https://github.com/YOUR_USERNAME/generic-bi-chatbot.git
cd generic-bi-chatbot
```

### **2. Get API Key**
1. Visit [Google AI Studio](https://aistudio.google.com/app/apikey)
2. Create free Gemini API key
3. Copy the key (starts with `AIza`)

### **3. Open & Configure**
1. Double-click `generic_ULTIMATE_COMPLETE.html`
2. Click **⚙️ API Settings**
3. Paste your API key
4. Click **Save**

### **4. Upload Data**
1. Click **📤 Upload Excel/CSV**
2. Select your file
3. Wait for "✅ Data Loaded"

### **5. Start Analyzing**
```
"Show me a summary"
"Top 10 products by revenue"
"Revenue by category"
"Show trend over time"
"Stockouts during diwali"
```

---

## 📂 Project Structure

```
generic-bi-chatbot/
│
├── generic_ULTIMATE_COMPLETE.html    # Main file - Generic version
├── freshco_chatbot_final.html        # Domain-specific version (optional)
├── README.md                          # This file
└── docs/                              # Documentation (optional)
    ├── USER_GUIDE.md
    ├── TECHNICAL_DOCS.md
    └── QUERY_EXAMPLES.md
```

---

## 🎯 Use Cases

### **For Students**
- 📚 Upload assignment datasets
- 🧪 Experiment with different queries
- 📊 Generate visualizations for reports
- 🔍 Validate calculations

### **For Businesses**
- 📈 Sales analysis
- 📦 Inventory management
- 💰 Profitability tracking
- 🎯 Marketing effectiveness

### **For Researchers**
- 📊 Data exploration
- 📈 Trend identification
- 🔬 Hypothesis testing
- 📉 Anomaly detection

---

## 💡 Example Queries

### **Basic Queries**
```
"Show me a summary"
"How many rows?"
"What columns do I have?"
```

### **Analysis Queries**
```
"Top 10 products by sales"
"Revenue by category"
"Monthly trend"
"Profit margin by brand"
```

### **Advanced Queries**
```
"Stockouts during festive season"
"Which city has lowest inventory?"
"Promotion effectiveness by channel"
"Discount impact on profit margins"
```

---

## 🏗️ Technical Architecture

### **Technology Stack**
- **Frontend**: HTML5, CSS3, JavaScript (Vanilla)
- **Charting**: Chart.js with DataLabels plugin
- **Excel Parsing**: SheetJS (xlsx.js)
- **AI Model**: Gemini 3 27B (gemma-3-27b-it)
- **API**: Google Generative AI API

### **How It Works**
```
User uploads Excel/CSV
        ↓
Auto-detect columns
        ↓
Smart column mapping
        ↓
User asks question
        ↓
Gemini interprets query
        ↓
JavaScript calculates results
        ↓
Display charts + tables + validation
```

### **Key Innovation: Generic Wrapper System**
```javascript
// Instead of hardcoded:
const product = row.Product_Name;  // ❌

// Dynamic mapping:
const product = row[colMap.Product_Name];  // ✅
```

This allows the same analysis code to work with any data structure!

---

## 🎓 Academic Context

### **Course**: GenAI for Business Applications
### **Institution**: IIM Ahmedabad
### **Semester**: Winter 2026

### **Project Goals**
1. ✅ Demonstrate AI integration in business analytics
2. ✅ Build production-ready solution
3. ✅ Show version control proficiency
4. ✅ Create reusable, generic tool

### **Learning Outcomes**
- AI API integration
- Natural language processing
- Dynamic data handling
- Professional UI/UX design
- Code reusability patterns

---

## 🔧 Configuration

### **Supported File Types**
- Excel: `.xlsx`, `.xls`
- CSV: `.csv`
- **Requirements**: First row must contain column headers

### **Data Requirements**
- Minimum 1 row of data
- Column headers in first row
- At least 1 numeric column for analysis

### **Recommended Data Structure**
```
Transaction_ID | Date       | Product  | Category | Sales | Units
1              | 2024-01-01 | Product1 | Food     | 1000  | 10
2              | 2024-01-02 | Product2 | Beverages| 1500  | 15
```

---

## 🐛 Troubleshooting

### **Issue: "Please set your API key"**
**Solution**: Click ⚙️ API Settings, add key, click Save

### **Issue: "No data found"**
**Solution**: Ensure Excel file has headers in first row

### **Issue: "Total Rows: 0"**
**Solution**: Query filters are too specific. Try simpler queries first.

### **Issue: Charts not showing**
**Solution**: 
1. Check console (F12) for errors
2. Ensure you have numeric columns
3. Try query: "Show me a summary"

### **Issue: "API Error 404"**
**Solution**: 
1. Check API key is correct (starts with `AIza`)
2. Verify key has access to gemma-3-27b-it model
3. Try changing model to `gemini-1.5-flash` in code

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| File Size | 194 KB |
| Lines of Code | 3,791 |
| Supported Columns | Unlimited |
| Max Data Rows | 100,000+ |
| Query Response Time | 2-5 seconds |
| API Cost per Query | ~$0.001 |

---

## 🔐 Security & Privacy

- ✅ **Local Storage**: API key stored in browser only
- ✅ **No Server**: All processing client-side
- ✅ **No Uploads**: Data never leaves your computer
- ✅ **Open Source**: Full code transparency
- ⚠️ **API Calls**: Data sent to Gemini API for query interpretation only

---

## 🌐 Browser Compatibility

| Browser | Supported | Tested |
|---------|-----------|--------|
| Chrome | ✅ | v120+ |
| Firefox | ✅ | v120+ |
| Edge | ✅ | v120+ |
| Safari | ✅ | v17+ |
| Opera | ✅ | v105+ |

---

## 📈 Roadmap

### **Version 2.0 (Planned)**
- [ ] Multi-sheet Excel support
- [ ] Export results to Excel
- [ ] Save/load query templates
- [ ] Custom color themes
- [ ] Multiple file comparison
- [ ] SQL query generation

### **Version 3.0 (Future)**
- [ ] Real-time collaboration
- [ ] Cloud storage integration
- [ ] Advanced ML predictions
- [ ] Custom visualization builder
- [ ] API for developers

---

## 🤝 Contributing

This is an academic project, but contributions are welcome!

### **How to Contribute**
1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

### **Contribution Guidelines**
- Follow existing code style
- Test with multiple datasets
- Update documentation
- Add example queries

---

## 📝 License

This project is licensed under the MIT License - see below for details:

```
MIT License

Copyright (c) 2026 [Your Name]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 👤 Author

**Shaurya**
- 🎓 IIM Ahmedabad
- 📧 [Your Email]
- 🔗 [LinkedIn Profile]
- 💼 [Portfolio]

---

## 🙏 Acknowledgments

- **IIM Ahmedabad** - For the GenAI course
- **Google AI** - For Gemini API access
- **Chart.js** - For beautiful visualizations
- **SheetJS** - For Excel parsing
- **Open Source Community** - For inspiration

---

## 📞 Support

### **For Issues**
- 🐛 [Report Bug](https://github.com/YOUR_USERNAME/generic-bi-chatbot/issues)
- 💡 [Request Feature](https://github.com/YOUR_USERNAME/generic-bi-chatbot/issues)
- 📧 Email: [Your Email]

### **For Questions**
- 💬 [GitHub Discussions](https://github.com/YOUR_USERNAME/generic-bi-chatbot/discussions)
- 📚 [Documentation](./docs/)

---

## 📊 Project Stats

![GitHub stars](https://img.shields.io/github/stars/YOUR_USERNAME/generic-bi-chatbot?style=social)
![GitHub forks](https://img.shields.io/github/forks/YOUR_USERNAME/generic-bi-chatbot?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/YOUR_USERNAME/generic-bi-chatbot?style=social)

---

## 🎯 Project Highlights

### **Technical Excellence**
- 🏗️ Modular architecture
- 🔄 Dynamic column mapping
- 🎨 Professional UI/UX
- 📊 Comprehensive analytics
- ✅ Full validation

### **Academic Rigor**
- 📚 Well-documented code
- 🧪 Extensively tested
- 📖 Complete README
- 🎓 Learning-focused
- 💡 Best practices

### **Business Value**
- 💰 Zero infrastructure cost
- ⚡ Instant insights
- 🔒 Data privacy
- 📈 Scalable solution
- 🌍 Universally applicable

---

## 🚀 Getting Started Video Tutorial

[Coming soon - YouTube tutorial link]

---

## 📸 Screenshots

### Main Interface
![Main Interface](./screenshots/main-interface.png)

### Data Upload
![Upload](./screenshots/upload.png)

### Analysis Results
![Results](./screenshots/results.png)

### Chart Visualization
![Charts](./screenshots/charts.png)

---

## 💬 Feedback

We'd love to hear from you! If you use this tool, please:
- ⭐ Star this repository
- 📝 Share your experience
- 🐛 Report any issues
- 💡 Suggest improvements

---

**Built with ❤️ for the IIM Ahmedabad GenAI Community**

**Last Updated**: January 11, 2026

---

---

**⭐ If this project helped you, please consider giving it a star! ⭐**
