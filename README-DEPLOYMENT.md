# Evolution API - Full Version Deployment

This repository contains the full Evolution API (not Lite) configured for Render deployment.

## Key Features (vs Lite Version)
- Manager UI at `/manager` endpoint
- Documentation endpoints
- Additional integrations and services
- Enhanced webhook and event management

## Deployment Configuration

### Environment Variables Required
All environment variables should be configured in your Render web service settings:

- `DATABASE_URL` - PostgreSQL connection string
- `REDIS_URI` - Redis connection string
- `AUTHENTICATION_API_KEY` - API key for authentication
- `DATABASE_PROVIDER` - Set to "postgresql"
- Other Evolution API configuration variables as needed

### Render Service Configuration
- **Build Command**: `npm install && npm run build`
- **Start Command**: `npm run start:prod`
- **Port**: The application will run on port 8080 (exposed in Dockerfile)

### Manager UI Access
Once deployed, the manager UI will be available at:
`https://your-render-service-url.onrender.com/manager`

### API Documentation
API documentation endpoints will be available at:
`https://your-render-service-url.onrender.com/`

## Differences from Lite Version
This full version includes:
- Complete manager interface
- Extended webhook capabilities
- Additional chatbot integrations
- Enhanced monitoring and event systems
- Full API documentation interface

## Migration from Lite Version
Simply update your Render web service to point to this repository instead of the lite version. All environment variables and database configurations remain the same.