# Weather Project Hub

Central repository for organizing and tracking development of weather-related applications and services.

## Project Components

| Repository | Description | Status |
|------------|-------------|--------|
| [Weather MCP Server](https://github.com/wasemag/weather-mcp) | MCP server providing weather data via Visual Crossing API | Active |
| [Weather Map App](https://github.com/wasemag/WeatherMapApp) | Web application displaying weather data on interactive maps | In Development |

## Architecture Overview

```
┌─────────────────┐      ┌───────────────────┐      ┌─────────────────┐
│                 │      │                   │      │                 │
│  Claude Desktop │◄────►│  Weather MCP      │◄────►│  Visual Crossing │
│                 │      │  Server           │      │  Weather API    │
│                 │      │                   │      │                 │
└────────┬────────┘      └────────┬──────────┘      └─────────────────┘
         │                        │
         │                        │
         │                        ▼
         │               ┌────────────────────┐
         │               │                    │
         └──────────────►│  Weather Map App   │
                         │                    │
                         └────────────────────┘
```

## Development Roadmap

### Current Phase
- Finalizing Weather MCP Server integration with Claude Desktop
- Developing the Weather Map App frontend

### Next Steps
- Add location search functionality to Weather Map App
- Implement alert visualization on map 
- Add historical data views
- Improve mobile responsiveness
- Create interactive weather dashboards

## Getting Started

To work with these projects locally:

1. Clone the repositories:
   ```bash
   git clone https://github.com/wasemag/weather-mcp.git
   git clone https://github.com/wasemag/WeatherMapApp.git
   ```

2. Set up the Weather MCP Server:
   - Follow instructions in the [Weather MCP README](https://github.com/wasemag/weather-mcp#installation)
   - Configure with your Visual Crossing API key

3. Set up the Weather Map App:
   - Follow instructions in the [Weather Map App README](https://github.com/wasemag/WeatherMapApp#docker-setup-instructions)
   - Ensure it's configured to connect to your Weather MCP Server instance

## Documentation

- [Visual Crossing API Documentation](https://www.visualcrossing.com/resources/documentation/weather-api/timeline-weather-api/)
- [Model Context Protocol (MCP) Overview](https://modelcontextprotocol.io/docs/concepts/architecture)