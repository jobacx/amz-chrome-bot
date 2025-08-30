# AMZ Chrome Bot

A comprehensive Chrome extension designed to automate and streamline Amazon Seller Central and Amazon.com operations. This powerful tool helps Amazon sellers extract data, manage inventory, monitor pricing, and perform various automation tasks across Amazon's ecosystem.

## 🚀 Key Features

### 📊 Data Extraction Tools

#### Amazon Detail Page Extraction
- **Product Information**: Extracts brand, title, ASIN, category, descriptions, and bullet points
- **Image Data**: Captures main product images with dimensions
- **Enhanced Content**: Retrieves EBC (Enhanced Brand Content) and A+ content
- **Sales Rank**: Extracts category rankings and sales data
- **One-Click Export**: Copies data to clipboard in tab-delimited format

#### Seller Central Inventory Management
- **Inventory Data**: SKU, status, ASIN, quantity, fulfillment channel
- **Price Monitoring**: Current prices, minimum/maximum price settings
- **Status Tracking**: Active/inactive listings, price alerts
- **Real-time Search**: Quick SKU/ASIN/UPC lookup functionality

#### Competitive Pricing Intelligence
- **Brand Health Data**: Extracts competitive pricing alerts from Brand Health page
- **Price Analysis**: Compares your prices vs. competitors
- **Market Insights**: Page views, conversion rates, competitiveness metrics
- **Excel Export**: Automatically generates detailed pricing reports

#### Price Alerts & Issues Management
- **Inactive Offers**: Listings deactivated due to pricing errors
- **Featured Offer Tracking**: Eligibility status and competitive positioning  
- **Sales Conversion**: Products with no sales and optimization suggestions
- **Automated Extraction**: Bulk processing with progress tracking

### 🔍 Product Detection & Monitoring

#### Velcro Detector
- **Brand Protection**: Automatically scans for "Velcro" trademark violations
- **Visual Highlighting**: Highlights found instances in yellow/red
- **Multi-section Scan**: Checks titles, bullets, descriptions, and EBC content
- **Instant Feedback**: Changes favicon and page title for quick identification

#### Image Quality Detector
- **Missing Image Detection**: Identifies products with no-image placeholders
- **Quality Assurance**: Ensures all listings have proper product images
- **Visual Indicators**: Changes favicon to show image status
- **Quick Navigation**: Works on offer-listing pages for rapid assessment

#### Add Product Intelligence
- **Duplicate Detection**: Identifies existing products during add process
- **Product Metrics**: UPC, EAN, sales rank, offer count extraction
- **Availability Status**: Checks product availability for selling
- **Bulk Processing**: Handles multiple product IDs simultaneously

### 🛠 Automation & Productivity Tools

#### Upload Feed Management
- **Purge & Replace Control**: Toggle dangerous bulk operations on/off
- **Smart Notifications**: Alerts when risky operations are enabled
- **Safety Features**: Hides accidental activation elements
- **Visual Warnings**: Color-coded status indicators

#### Bulk Data Processing
- **Multi-format Support**: Handles ASIN, UPC, EAN, and SKU inputs
- **Batch Operations**: Process up to 100 products simultaneously
- **Progress Tracking**: Real-time status updates during bulk operations
- **Tab Management**: Automatic opening and closing of processing tabs

#### Navigation & Search Enhancement
- **Quick Search**: Instant navigation to specific Amazon pages
- **Keyboard Shortcuts**: Extensive hotkey support for power users
- **Tab Organization**: Copy all tab URLs, bulk tab management
- **Smart Routing**: Context-aware page detection and tool activation

## 🏗 Technical Architecture

### Tech Stack
- **Framework**: Chrome Extension Manifest V2
- **Frontend**: HTML5, CSS3 with W3.CSS framework  
- **JavaScript**: ES6+ with jQuery 3.x
- **Data Processing**: XLSX.js for Excel file generation
- **Styling**: Custom CSS with responsive design
- **Storage**: Chrome Extension local storage API

### Core Technologies

#### JavaScript Libraries
- **jQuery 3.x**: DOM manipulation and AJAX requests
- **XLSX.js**: Excel file creation and export functionality
- **jQuery Table2Excel**: Table-to-Excel conversion utility

#### Chrome Extension APIs
- **Tabs API**: Tab management and navigation
- **Storage API**: Settings and data persistence  
- **Notifications API**: Desktop notification system
- **Content Scripts**: Page interaction and data extraction
- **Background Scripts**: Event handling and cross-tab communication

#### Data Formats
- **JSON**: Configuration and data storage
- **Excel (XLSX)**: Report generation and data export
- **Tab-delimited**: Clipboard data formatting
- **CSV**: Alternative export format support

### Extension Structure

```
amz-chrome-bot/
├── manifest.json          # Extension configuration
├── background.js           # Background event handling
├── content.js             # Main content script injection
├── popup.html/js          # Extension popup interface
├── options.html/js        # Settings and bulk operations
├── js/
│   ├── myscript.js        # Core utility functions
│   ├── velcroDetector.js  # Trademark violation detection
│   ├── noImgDetector.js   # Image quality monitoring
│   ├── addProductExtractor.js # Product addition intelligence
│   ├── priceIssues.js     # Price alert management
│   └── xlsx.full.min.js   # Excel generation library
├── css/                   # Styling and themes
└── images/               # Extension icons and assets
```

## ⌨️ Keyboard Shortcuts

- **Ctrl+Shift+Space**: Open extension popup
- **Ctrl+1-6**: Navigate between extension menus
- **Ctrl+Enter**: Extract data from current page
- **Ctrl+Left Arrow**: Navigate to product detail page
- **Ctrl+Right Arrow**: Navigate to offer-listing page

## 🎯 Use Cases

### Amazon Seller Operations
- Monitor competitor pricing and adjust strategies
- Extract product data for catalog management
- Automate inventory status monitoring
- Bulk process new product additions
- Track price alert notifications

### Quality Assurance
- Scan listings for trademark violations
- Verify product images are present and proper
- Check product data completeness
- Monitor listing health across catalog

### Market Research
- Extract competitor product information
- Analyze pricing trends and strategies
- Research product categories and rankings
- Export data for external analysis tools

### Compliance & Brand Protection
- Monitor unauthorized use of trademarks
- Track listing quality metrics
- Ensure brand guideline adherence
- Automate compliance checking workflows

## 📋 Version History

### Latest Updates (v2.2.2)
- Enhanced Brand Health page data extraction
- Improved competitive pricing intelligence
- Updated Price Alert page extractors
- Fixed Seller Central compatibility issues
- Added bulk processing improvements

### Historical Milestones
- **2020**: Initial Amazon detail page extraction
- **2021**: Added Brand Health and competitive data tools
- **2022**: Enhanced pricing health monitoring features

## 🔒 Permissions & Security

The extension requires the following permissions:
- **tabs**: Tab management and navigation
- **storage**: Save settings and extracted data
- **notifications**: Desktop alerts and updates
- **activeTab**: Access current tab content
- **https://*/***: Access Amazon and Seller Central pages

All data processing occurs locally within the browser. No personal or business data is transmitted to external servers.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### MIT License Summary
- ✅ **Commercial use** - Use for commercial purposes
- ✅ **Modification** - Modify the source code  
- ✅ **Distribution** - Distribute copies of the software
- ✅ **Private use** - Use for private purposes
- ❗ **Limitation of liability** - No warranty or liability
- ❗ **License and copyright notice** - Include license in copies
