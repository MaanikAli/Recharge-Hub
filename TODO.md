# Login System Debug and Test

## Steps to Debug Login Issue

1. **Install Backend Dependencies**
   - Navigate to backend directory
   - Run `npm install` to ensure all packages are installed

2. **Start MongoDB**
   - Ensure MongoDB is running locally (default port 27017)
   - If not, start MongoDB service

3. **Start Backend Server**
   - In backend directory, run `npm run dev` or `npm start`
   - Check console for "Server running on port 5000" and "MongoDB connected"
   - Verify preset admin is created

4. **Install Frontend Dependencies**
   - In root directory, run `npm install`

5. **Start Frontend Development Server**
   - Run `npm run dev` (assuming Vite)
   - Open browser to localhost:3000 or specified port

6. **Test Login Functionality**
   - Attempt login with username: 'tarek', password: 'tarek123'
   - Check browser console for errors
   - Check network tab for API request/response
   - Check backend console for logs

7. **Identify and Fix Issues**
   - If login fails, check:
     - Backend server running
     - MongoDB connection
     - API endpoint reachable
     - Credentials correct
     - CORS issues
     - JWT token generation/storage

8. **Verify Successful Login**
   - After successful login, should redirect to dashboard
   - Token stored in localStorage
   - Subsequent API calls include Authorization header
