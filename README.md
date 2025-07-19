# SmelterXplore™ - Heatmap Quality Monitoring System

## Overview
SmelterXplore™ is a comprehensive digital dashboard system designed for monitoring and visualizing quality metrics across Smelter & Refinery processing locations. The system provides real-time heatmap visualization based on laboratory sampling data, enabling rapid detection of quality deviations and informed decision-making.

## Features

### 🎯 Core Dashboard Sections
- **Dashboard Overview**: Real-time heatmap visualization of all processing locations
- **Reports**: Comprehensive data management with export capabilities
- **Locations**: Detailed analysis of individual processing locations
- **History**: Historical data trends with date range filtering
- **Alerts**: Quality deviation notifications and critical alerts
- **Analytics**: Advanced charts and performance insights

### 🔐 Authentication & Security
- Secure login system (username: kanghaji, password: 475400)
- Session management with local storage
- Protected routes for authenticated users only

### 📊 Data Input Methods
- **Manual Input**: Form-based data entry for quality samples
- **Barcode Scanning**: Simulated barcode scanning functionality
- **File Upload**: CSV/Excel/PDF document upload capability

### 🎨 Modern UI Features
- Responsive design for desktop and mobile devices
- Dark/light theme toggle
- Interactive heatmap with color-coded quality indicators
- Real-time data updates
- Modern, eye-catching design with SmelterXplore™ branding

## Processing Locations & Quality Targets

| Location | Product | Target Quality | Unit |
|----------|---------|----------------|------|
| DISCHARGE POINT | Copper Concentrate | 25% | % |
| FLASH SMELTING FURNACE | Copper Matte | 70% | % |
| SLAG CONCENTRATOR | Recovery Copper Concentrate | 22% | % |
| ACID PLANT | Sulfuric Acid | 98.5% | % |
| FLASH CONVERTING FURNACE | Copper Blister | 98.5% | % |
| ANODE FURNACE & ANODE CASTING WHEEL | Copper Anode | 99.2% | % |
| COPPER ELECTRO REFINING | Copper Cathode | 99.99% | % |
| PMR GOLD | Gold | 99.99% | % |
| PMR SILVER | Silver | 99.99% | % |

## Technology Stack

- **Frontend**: Next.js 15.3.2 with TypeScript
- **Styling**: Tailwind CSS v4 with shadcn/ui components
- **Charts**: Recharts for data visualization
- **State Management**: React hooks with local storage
- **Icons**: Lucide React
- **Notifications**: Sonner toast notifications

## Installation & Setup

1. **Clone the repository**
   ```bash
   git clone [repository-url]
   cd smelterxplore
   ```

2. **Install dependencies**
   ```bash
   npm install --legacy-peer-deps
   ```

3. **Start the development server**
   ```bash
   npm run dev
   ```

4. **Access the application**
   - Open http://localhost:8000 in your browser
   - Login with credentials: username: kanghaji, password: 475400

## Usage Guide

### Initial Setup
1. The application automatically generates 50 sample data points for each processing location
2. Data is stored in browser local storage for persistence
3. All features are fully functional without external dependencies

### Dashboard Navigation
- **Home**: Overview of all processing locations with heatmap visualization
- **Reports**: Add new samples and export data in CSV/JSON formats
- **Locations**: Detailed view of individual processing locations
- **History**: Filter historical data by date range
- **Alerts**: Monitor quality deviations and critical alerts
- **Analytics**: Advanced charts and performance metrics
- **Settings**: Configure application preferences

### Data Management
- **Adding Samples**: Use the Reports page to add new quality samples
- **Export Data**: Export complete datasets in CSV or JSON format
- **Clear Data**: Reset all sample data from Settings page

## Data Structure

Each quality sample contains:
- Sample ID (unique identifier)
- Processing location reference
- Quality value with unit
- Status (PASS/WARNING/FAIL)
- Timestamp
- Operator information
- Batch number
- Test method
- Additional notes

## Heatmap Color Coding

- **Green (#22c55e)**: Excellent quality (within 20% of target)
- **Yellow (#eab308)**: Good quality (within 50% of target)
- **Orange (#f97316)**: Warning quality (within 80% of target)
- **Red (#ef4444)**: Critical quality (beyond acceptable range)

## Future Enhancements

- Integration with LIMS (Laboratory Information Management System)
- ERP system connectivity
- Real-time data streaming
- Advanced predictive analytics
- Mobile application
- Multi-user role management
- API endpoints for external integrations

## Support & Maintenance

For technical support or feature requests, please contact the development team.

## License

This project is proprietary software developed for Smelter & Refinery quality monitoring applications.
