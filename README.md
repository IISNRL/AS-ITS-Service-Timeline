# AS-ITS Service Timeline

A visual timeline application for tracking and displaying service events in an interactive and user-friendly format.

[![Demo](https://img.shields.io/badge/Demo-Live-brightgreen)](https://aws.cclljj.net/AS-ITS/AS-ITS-Service-Timeline/)

## Demo

View the live demonstration: [AS-ITS Service Timeline Demo](https://aws.cclljj.net/AS-ITS/AS-ITS-Service-Timeline/)

## Overview

This application renders an interactive timeline visualization from event data stored in CSV format. Users can filter events by type and view detailed information about each event. The timeline uses color-coding to distinguish between different event categories, providing an intuitive visual representation of service history.

## Features

- **Interactive Timeline**: Navigate through time with zoom and pan capabilities
- **Event Filtering**: Filter events by type, category, or custom attributes
- **Color-Coded Categories**: Quickly identify event types through visual indicators
- **Responsive Design**: Optimized for desktop, tablet, and mobile displays
- **Event Details**: Access comprehensive information by hovering or clicking events
- **Data-Driven**: Easily update by modifying the CSV data source

## Project Structure

```
AS-ITS-Service-Timeline/
├── index.html           # Main HTML entry point
├── src/
│   └── timeline.js      # Core timeline rendering and interaction logic
├── style/
│   └── timeline.css     # Timeline styling and responsive design rules
├── data/
│   └── events.csv       # Event data in CSV format
└── README.md            # Project documentation
```

## Installation

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- Basic knowledge of HTML/CSS/JavaScript for customization

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/AS-ITS-Service-Timeline.git
   cd AS-ITS-Service-Timeline
   ```

2. No build process is required. You can:
   - Open `index.html` directly in a web browser
   - Host using a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js (after installing http-server)
     npx http-server
     ```

3. For production deployment, upload all files to your web server.

## Configuration

### Event Data Format

The `data/events.csv` file should follow this format:

```csv
id,start,end,content,type,className
1,2023-04-01,2023-04-03,System Maintenance,maintenance,maintenance-event
2,2023-04-15,,Service Launch,milestone,milestone-event
```

Fields:
- `id`: Unique identifier for the event
- `start`: Start date (YYYY-MM-DD) or datetime (YYYY-MM-DD HH:MM:SS)
- `end`: End date/time (leave empty for point events)
- `content`: Title/description of the event
- `type`: Event category (maintenance, milestone, incident, etc.)
- `className`: CSS class for custom styling

### Customization

- **Styling**: Modify `style/timeline.css` to change colors, fonts, and layout
- **Behavior**: Adjust timeline parameters in `src/timeline.js`
- **Extensions**: Add new features by extending the timeline.js functionality

## Browser Compatibility

- Chrome (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Edge (latest 2 versions)

## Dependencies

- [vis-timeline](https://visjs.github.io/vis-timeline/) - Dynamic, browser-based visualization library

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Maintenance

This project is actively maintained. If you encounter any issues or have suggestions, please open an issue in the repository.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

Project Maintainer - [Your Name](mailto:your.email@example.com)

Project Link: [https://github.com/yourusername/AS-ITS-Service-Timeline](https://github.com/yourusername/AS-ITS-Service-Timeline)