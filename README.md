# HelpHub - Helplytics

Full-stack application with monorepo structure.

## Project Structure

```
├── backend/      # Node.js/Express API server
├── frontend/     # Next.js React application
└── vercel.json   # Vercel deployment config
```

## Backend

Express.js API server with MongoDB integration.

- **Port**: 5000 (default)
- **Tech**: Node.js, Express, MongoDB, JWT Auth

```bash
cd backend
npm install
npm run dev    # Development with nodemon
npm start      # Production
```

## Frontend

Next.js React application with Tailwind CSS.

- **Port**: 3000 (default)
- **Tech**: Next.js 14, React 18, Tailwind CSS

```bash
cd frontend
npm install
npm run dev    # Development
npm run build  # Production build
npm start      # Production server
```

## Deployment

**Frontend**: Deployed on Vercel  
**Backend**: Can be deployed on Render, Railway, or Vercel Functions

For Vercel, the `vercel.json` at root configures the frontend as the deployment target.

## Environment Variables

### Backend (.env)
```
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

### Frontend (.env.local)
```
NEXT_PUBLIC_API_URL=your_backend_api_url
```
