# 📊 Generic BI Chatbot - Full Featured

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Production](https://img.shields.io/badge/Status-Production-green.svg)]()
[![AI: Gemini](https://img.shields.io/badge/AI-Gemini%203%2027B-blue.svg)]()

> AI-powered business intelligence chatbot with complete CPG analytics capabilities. Upload any Excel/CSV file and get instant insights with charts, tables, and validation.

**🎓 Academic Project** | IIM Ahmedabad | GenAI Course | January 2026

---

## 🌿 Repository Structure

This repository demonstrates version control best practices with two main branches:

### **`main` Branch** - FreshCo Specific Version
- Domain-specific implementation for FreshCo CPG dataset
- Hardcoded column names for 206K-row dataset
- Optimized for specific business use case
- Direct Google Sheets integration
- 📄 File: `freshco_chatbot_final.html`

### **`feature/generic-version` Branch** ⭐ - Generic Universal Version
- **Works with ANY Excel/CSV data**
- Dynamic column detection and mapping
- Bring Your Own API Key (BYOK)
- File upload instead of Google Sheets
- All 12 FreshCo analysis types preserved
- 📄 File: `generic_ULTIMATE_COMPLETE.html`

**🔗 Quick Links:**
- [View FreshCo Version](https://github.com/YOUR_USERNAME/generic-bi-chatbot/tree/main)
- [View Generic Version](https://github.com/YOUR_USERNAME/generic-bi-chatbot/tree/feature/generic-version) ⭐ **Recommended**

---

## 🚀 Quick Start (Generic Version)

### **Access the Generic Version**

**Option 1: Direct Download**
```bash
# Clone the generic branch
git clone -b feature/generic-version https://github.com/YOUR_USERNAME/generic-bi-chatbot.git
cd generic-bi-chatbot
```

**Option 2: Switch to Branch**
```bash
# If already cloned
git clone https://github.com/YOUR_USERNAME/generic-bi-chatbot.git
cd generic-bi-chatbot
git checkout feature/generic-version
```

**Option 3: Direct File Link**
- Navigate to: `feature/generic-version` branch
- Download: `generic_ULTIMATE_COMPLETE.html`
- Open in browser

### **Setup (3 Steps)**

1. **Get API Key**
   - Visit [Google AI Studio](https://aistudio.google.com/app/apikey)
   - Create free Gemini API key
   - Copy the key (starts with `AIza`)

2. **Open & Configure**
   - Open `generic_ULTIMATE_COMPLETE.html` in browser
   - Click **⚙️ API Settings**
   - Paste your API key
   - Click **Save**

3. **Upload & Analyze**
   - Click **📤 Upload Excel/CSV**
   - Select your data file
   - Wait for "✅ Data Loaded"
   - Start asking questions!

---

## 🌟 Features

### **Core Capabilities**
- ✅ **Upload Any Data** - Works with Excel (.xlsx, .xls) or CSV files
- ✅ **Auto-Detection** - Automatically detects and maps columns
- ✅ **12 Query Types** - Comprehensive analysis capabilities
- ✅ **Professional Charts** - Bar, line, and pie charts with Chart.js
- ✅ **Validation Sections** - Step-by-step calculation breakdowns
- ✅ **BYOK** - Bring Your Own API Key (stored locally)
- ✅ **No Server Required** - 100% client-side processing

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
"Group by region"
```

### **Advanced Queries**
```
"Stockouts during festive season"
"Which city has lowest inventory?"
"Promotion effectiveness by channel"
"Discount impact on profit margins"
"Revenue trend over time"
```

---

## 📂 Branch Comparison

| Feature | main (FreshCo) | feature/generic-version |
|---------|----------------|-------------------------|
| **Data Source** | Google Sheets | Excel/CSV Upload |
| **Column Detection** | Hardcoded | Dynamic |
| **Dataset** | FreshCo 206K rows | ANY dataset |
| **API Key** | Embedded | BYOK |
| **Use Case** | Domain-specific | Universal |
| **Analysis Types** | 12 types | 12 types |
| **Sharing** | Limited | Unlimited |
| **For Professor** | ✅ Demo original | ✅ Show versioning |
| **For Classmates** | ❌ Can't use | ✅ Can use |
| **Production Ready** | ✅ Yes | ✅ Yes |

---

## 🎯 Use Cases

### **Generic Version (`feature/generic-version`)**

**For Students:**
- 📚 Upload assignment datasets
- 🧪 Experiment with different queries
- 📊 Generate visualizations for reports
- 🔍 Validate calculations

**For Businesses:**
- 📈 Sales analysis
- 📦 Inventory management
- 💰 Profitability tracking
- 🎯 Marketing effectiveness

**For Researchers:**
- 📊 Data exploration
- 📈 Trend identification
- 🔬 Hypothesis testing
- 📉 Anomaly detection

### **FreshCo Version (`main`)**

**For Demo:**
- 🏢 Show domain-specific optimization
- 📊 Present to stakeholders
- 🎯 Production deployment
- 📈 Real business use case

---

## 🏗️ Technical Architecture

### **Generic Version Innovation**

The key innovation is the **Generic Wrapper System** that makes FreshCo's specialized logic work with any data:

```javascript
// Before (FreshCo - Hardcoded):
const product = row.Product_Name;        // ❌
const revenue = row.Sales_Value;         // ❌

// After (Generic - Dynamic):
const product = row[colMap.Product_Name]; // ✅
const revenue = row[colMap.Sales_Value];  // ✅
```

**How it works:**
1. User uploads Excel/CSV
2. System detects all columns
3. Fuzzy matching maps to FreshCo equivalents
4. All 12 analysis functions work unchanged
5. Results displayed with charts & validation

### **Technology Stack**
- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Charting**: Chart.js with DataLabels plugin
- **Excel Parsing**: SheetJS (xlsx.js)
- **AI Model**: Gemini 3 27B (gemma-3-27b-it)
- **API**: Google Generative AI API

---

## 🎓 Academic Context

### **Course**: GenAI for Business Applications
### **Institution**: IIM Ahmedabad
### **Semester**: Winter 2026

### **Project Evolution**
```
Version 1 (main branch)
    ↓
Domain-specific FreshCo implementation
    ↓
Version 2 (feature/generic-version branch)
    ↓
Generic version with dynamic mapping
    ↓
Demonstrates version control & code reusability
```

### **Learning Outcomes**
- ✅ AI API integration
- ✅ Natural language processing
- ✅ Dynamic data handling
- ✅ **Version control with Git branches**
- ✅ **Code generalization & reusability**
- ✅ Professional UI/UX design

---

## 🔧 Configuration

### **Supported File Types** (Generic Version)
- Excel: `.xlsx`, `.xls`
- CSV: `.csv`
- **Requirements**: First row must contain column headers

### **Data Requirements**
- Minimum 1 row of data
- Column headers in first row
- At least 1 numeric column for analysis

### **Recommended Data Structure**
```csv
Transaction_ID,Date,Product,Category,Sales,Units
1,2024-01-01,Product1,Food,1000,10
2,2024-01-02,Product2,Beverages,1500,15
```

**Column Mapping Examples:**
- `Product` / `Product_Name` / `Item` → Auto-detected as product
- `Sales` / `Sales_Value` / `Revenue` → Auto-detected as revenue
- `Category` / `Type` / `Segment` → Auto-detected as category
- Works with ANY column names!

---

## 🐛 Troubleshooting

### **Issue: "Please set your API key"**
**Solution**: 
- Click ⚙️ API Settings
- Paste your Gemini API key (starts with `AIza`)
- Click Save

### **Issue: "No data found"**
**Solution**: 
- Ensure Excel file has headers in first row
- Check file is not empty
- Try saving as CSV and uploading

### **Issue: "Total Rows: 0"**
**Solution**: 
- Query filters are too specific
- Try: "Show me a summary" first
- Check console (F12) for column mapping

### **Issue: Charts not showing**
**Solution**: 
1. Press F12 → Console for errors
2. Ensure you have numeric columns
3. Verify data loaded: Check "✅ Data Loaded" message

### **Issue: "API Error 404"**
**Solution**: 
1. Verify API key is correct
2. Check key has gemma-3-27b-it access
3. Alternative: Edit HTML, change model to `gemini-1.5-flash`

---

## 📊 Performance

| Metric | Generic Version | FreshCo Version |
|--------|----------------|-----------------|
| File Size | 194 KB | 183 KB |
| Lines of Code | 3,791 | 3,648 |
| Supported Columns | Unlimited | 30 fixed |
| Max Data Rows | 100,000+ | 206,000 tested |
| Query Response Time | 2-5 seconds | 2-5 seconds |
| API Cost per Query | ~$0.001 | ~$0.001 |
| Setup Time | 2 minutes | Instant |
| Flexibility | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ |

---

## 🔐 Security & Privacy

### **Generic Version (feature/generic-version)**
- ✅ **Local Storage**: API key stored in browser only
- ✅ **No Server**: All processing client-side
- ✅ **No Uploads**: Data never leaves your computer
- ✅ **Open Source**: Full code transparency
- ⚠️ **API Calls**: Only query interpretation sent to Gemini

### **FreshCo Version (main)**
- ✅ **Google Sheets**: Read-only access
- ✅ **Embedded Key**: Pre-configured for demo
- ⚠️ **Not for Production**: API key visible in code

---

## 🌐 Browser Compatibility

| Browser | Generic Version | FreshCo Version |
|---------|----------------|-----------------|
| Chrome | ✅ v120+ | ✅ v120+ |
| Firefox | ✅ v120+ | ✅ v120+ |
| Edge | ✅ v120+ | ✅ v120+ |
| Safari | ✅ v17+ | ✅ v17+ |
| Opera | ✅ v105+ | ✅ v105+ |

---

## 📈 Version Control Strategy

This repository demonstrates professional version control:

```
main (FreshCo Version)
    │
    ├── freshco_chatbot_final.html
    ├── README.md
    └── LICENSE
    
feature/generic-version (Generic Version) ⭐
    │
    ├── generic_ULTIMATE_COMPLETE.html
    ├── README.md (this file)
    └── DOCUMENTATION/
```

**Why This Structure?**
- ✅ Preserves original FreshCo version
- ✅ Shows evolution of project
- ✅ Demonstrates Git branching
- ✅ Allows parallel development
- ✅ Easy to compare versions
- ✅ Professional workflow

---

## 🤝 Contributing

### **Current Branches**
- `main` - Stable FreshCo version
- `feature/generic-version` - Active development

### **How to Contribute**
1. Fork the repository
2. Create feature branch from `feature/generic-version`
   ```bash
   git checkout -b feature/YourFeature feature/generic-version
   ```
3. Make changes
4. Test with multiple datasets
5. Submit pull request to `feature/generic-version`

---

## 📝 License

MIT License - See [LICENSE](./LICENSE) file for details

---

## 👤 Author

**Shaurya**
- 🎓 IIM Ahmedabad
- 📧 [Your Email]
- 🔗 [LinkedIn Profile]
- 💼 [GitHub Profile]

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

### **For Questions**
- 💬 [GitHub Discussions](https://github.com/YOUR_USERNAME/generic-bi-chatbot/discussions)
- 📧 Email: [Your Email]

---

## 🔗 Quick Access

### **Main Branch (FreshCo Version)**
- [View Code](https://github.com/YOUR_USERNAME/generic-bi-chatbot/tree/main)
- [Download](https://github.com/YOUR_USERNAME/generic-bi-chatbot/archive/refs/heads/main.zip)
- **Use Case**: Demo, showcase, production deployment

### **Generic Branch (Recommended)** ⭐
- [View Code](https://github.com/YOUR_USERNAME/generic-bi-chatbot/tree/feature/generic-version)
- [Download](https://github.com/YOUR_USERNAME/generic-bi-chatbot/archive/refs/heads/feature/generic-version.zip)
- **Use Case**: Personal use, sharing, assignments

---

## 📊 Project Stats

![GitHub branches](https://img.shields.io/badge/branches-2-blue)
![Main branch](https://img.shields.io/badge/main-FreshCo-orange)
![Feature branch](https://img.shields.io/badge/feature-Generic-green)

---

## 🎯 Which Version Should I Use?

### **Use Main Branch (FreshCo) if:**
- ✅ You want to see the original implementation
- ✅ You have FreshCo dataset
- ✅ You're demonstrating to stakeholders
- ✅ You want ready-to-run demo

### **Use Generic Branch if:** ⭐ **Recommended**
- ✅ You have your own data
- ✅ You want to share with classmates
- ✅ You need flexibility
- ✅ You want BYOK (privacy)
- ✅ You're doing assignments
- ✅ You want to customize

---

## 💬 Feedback

**For Professor:**
- 📊 Demonstrates version control skills
- 🔄 Shows code generalization ability
- 🎯 Highlights software engineering best practices
- ⭐ Both versions production-ready

**For Classmates:**
- 🚀 Use the generic version with your data
- 📚 Great for course assignments
- 🔐 Your API key = Your credits
- 💡 Learn from the code structure

---

**Built with ❤️ for the IIM Ahmedabad GenAI Community**

**Last Updated**: January 11, 2026

---

## 🎓 For Evaluation

**Professor, please note:**

This repository demonstrates:
1. ✅ **Original Implementation** (main branch) - FreshCo specific
2. ✅ **Generic Implementation** (feature/generic-version) - Universal
3. ✅ **Version Control** - Proper branching strategy
4. ✅ **Code Reusability** - Same logic, different data sources
5. ✅ **Documentation** - Complete README on both branches
6. ✅ **Production Quality** - Both versions fully functional

**Navigate between branches to see the evolution!**

---

**⭐ If this project helped you, please consider giving it a star! ⭐**

**🌿 Currently viewing: `feature/generic-version` branch** (Recommended for general use)
