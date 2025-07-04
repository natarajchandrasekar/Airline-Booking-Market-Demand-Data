# 🛫 Airline Market Demand Analytics - Setup Guide

## 📋 Overview
This web application provides comprehensive analysis of airline booking market demand data with AI-powered insights using Gemini 1.5 Flash API. The app is built with Streamlit for a professional, user-friendly interface.

## 🚀 Quick Start

### 1. Prerequisites
- Python 3.8 or higher
- pip package manager
- Internet connection for API calls

### 2. Installation

1. **Clone or Download the Project**
   ```bash
   # Create a new directory
   mkdir airline-demand-app
   cd airline-demand-app
   ```

2. **Save the Files**
   - Save the main application code as `airline_app.py`
   - Save the requirements as `requirements.txt`

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Application**
   ```bash
   streamlit run airline_app.py
   ```

5. **Access the App**
   - Open your web browser
   - Go to `http://localhost:8501`

## 🔑 API Configuration

### Getting Your Gemini API Key

1. **Visit Google AI Studio**
   - Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
   - Sign in with your Google account

2. **Create API Key**
   - Click "Create API Key"
   - Choose your project or create a new one
   - Copy the generated API key

3. **Configure in App**
   - Enter your API key in the sidebar
   - You'll see a "✅ API Key successfully configured!" message

### Without API Key
- The app works without an API key
- Uses simulated AI analysis instead of real Gemini insights
- All other features remain fully functional

## 🎯 Key Features

### 1. Data Analysis
- **Route Analysis**: Popular routes, booking volumes, demand scores
- **Price Trends**: 30-day price movements, airline comparisons
- **Demand Patterns**: Seasonal variations, peak periods

### 2. AI-Powered Insights
- Intelligent market analysis using Gemini 1.5 Flash
- Business recommendations
- Risk assessment and opportunities
- Professional reporting format

### 3. Interactive Visualizations
- Bar charts for route popularity
- Line charts for price trends
- Scatter plots for price vs demand correlation
- Pie charts for demand distribution
- Heat maps for seasonal patterns

### 4. Professional UI
- Clean, modern design
- Responsive layout
- Intuitive navigation
- Mobile-friendly interface

### 5. Data Export
- CSV export for all data tables
- Download route data, price trends, and demand patterns
- Easy integration with Excel and other tools

## 🛠️ Technical Architecture

### Data Layer
- **Simulated Data Generator**: Creates realistic airline booking data
- **Data Processing**: Pandas for data manipulation and analysis
- **Export Functionality**: CSV generation for external use

### AI Integration
- **Gemini 1.5 Flash**: Advanced AI analysis and insights
- **Fallback Analysis**: Works without API key
- **Error Handling**: Graceful degradation if API fails

### Visualization Layer
- **Plotly**: Interactive charts and graphs
- **Streamlit**: Web interface and user interaction
- **Custom CSS**: Professional styling and branding

## 📊 Data Sources

### Current Implementation
- **Simulated Data**: Realistic airline booking patterns
- **Australian Focus**: Major cities and routes
- **Multiple Airlines**: Qantas, Virgin Australia, Emirates, etc.

### Future Enhancements
- **Real API Integration**: Amadeus, Sabre, or other travel APIs
- **Live Data Feeds**: Real-time booking information
- **Web Scraping**: Public airline websites (with proper permissions)

## 🔧 Customization Options

### Adding New Cities
```python
# In the AirlineDataSimulator class
self.cities = [
    "Sydney", "Melbourne", "Brisbane", "Perth", "Adelaide", 
    "Your_New_City"  # Add here
]
```

### Adding New Airlines
```python
# In the AirlineDataSimulator class
self.airlines = [
    "Qantas", "Virgin Australia", "Emirates",
    "Your_New_Airline"  # Add here
]
```

### Modifying Analysis Parameters
```python
# Generate more routes
route_data = data_simulator.generate_route_data(num_routes=100)

# Extend price trend period
price_data = data_simulator.generate_price_trends(days=60)
```

## 🚨 Troubleshooting

### Common Issues

1. **Streamlit Not Found**
   ```bash
   pip install streamlit
   ```

2. **Import Errors**
   ```bash
   pip install -r requirements.txt --upgrade
   ```

3. **Port Already in Use**
   ```bash
   streamlit run airline_app.py --server.port 8502
   ```

4. **API Key Issues**
   - Ensure your API key is correct
   - Check Google AI Studio for quota limits
   - Verify internet connection

### Performance Tips
- Use city filters to reduce data processing
- Clear browser cache if charts don't load
- Refresh the page if data doesn't update

## 📈 Business Value

### For Hostel Operators
- **Market Intelligence**: Understand travel patterns to your cities
- **Pricing Strategy**: Optimize hostel rates based on flight prices
- **Demand Forecasting**: Predict busy periods for better planning
- **Route Analysis**: Identify new markets and opportunities

### Competitive Advantages
- **Real-time Insights**: Stay ahead of market changes
- **Data-driven Decisions**: Make informed business choices
- **Professional Presentation**: Impress stakeholders with quality analysis
- **Scalable Solution**: Easy to expand to new markets

## 🔮 Future Enhancements

### Planned Features
1. **Real Data Integration**: Connect to live airline APIs
2. **Machine Learning**: Predictive analytics for demand forecasting
3. **Advanced Filtering**: More granular data selection
4. **Alert System**: Notifications for significant market changes
5. **Multi-language Support**: International market analysis

### Technical Improvements
1. **Database Integration**: PostgreSQL or MongoDB for data storage
2. **Caching**: Redis for improved performance
3. **Authentication**: User management and access control
4. **Deployment**: Docker containers and cloud hosting

