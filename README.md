# URL Shortener Project

This project is a feature-rich URL shortener application with user authentication, QR code generation, custom URLs, and click statistics. The application allows users to shorten long URLs, customize the short URLs, generate QR codes for the shortened URLs, and track click statistics, including the location and device type of the users.

## Features

- **User Authentication**: Secure user registration and login functionality.
- **URL Shortening**: Shorten long URLs to create easy-to-share links.
- **Custom URLs**: Users can create custom short URLs.
- **QR Code Generation**: Generate QR codes for each shortened URL.
- **Click Statistics**: Track and display statistics about the clicks on the shortened URLs, including:
  - Location of the users.
  - Device type (mobile, desktop, tablet).

## Tech Stack

- **Frontend**: React, Vite
- **Backend**: Node.js, Express
- **Database**: Supabase
- **Authentication**: Supabase Auth
- **Storage**: Supabase Storage
- **QR Code Generation**: `react-qrcode-logo`

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/your-username/url-shortener.git
    ```
2. Navigate to the project directory:
    ```sh
    cd url-shortener
    ```
3. Install dependencies:
    ```sh
    npm install
    ```

## Configuration

1. Set up a Supabase project and obtain the necessary keys.
2. Create a `.env` file in the root directory and add your Supabase credentials:
    ```env
    REACT_APP_SUPABASE_URL=your-supabase-url
    REACT_APP_SUPABASE_ANON_KEY=your-supabase-anon-key
    ```

## Usage

1. Start the development server:
    ```sh
    npm run dev
    ```
2. Open your browser and navigate to `http://localhost:3000`.

## Project Structure

- `src/components`: Contains reusable UI components.
- `src/pages`: Contains page components like Landing, Dashboard, Auth, and Redirect.
- `src/hooks`: Custom hooks for data fetching and state management.
- `src/context`: Context providers for managing global state.
- `src/db`: API functions for interacting with Supabase.

## API Endpoints

- **POST /api/shorten**: Shorten a new URL.
- **GET /api/stats**: Retrieve statistics for a shortened URL.
- **GET /:id**: Redirect to the original URL.

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) before submitting a pull request.

## Acknowledgments

- [Supabase](https://supabase.io/) for the backend services.
- [React](https://reactjs.org/) for the frontend framework.
- [Vite](https://vitejs.dev/) for the build tool.

Feel free to explore, use, and contribute to the project. If you encounter any issues or have any suggestions, please open an issue on GitHub.

---

**Note**: Replace placeholder URLs and keys with actual values from your project.
