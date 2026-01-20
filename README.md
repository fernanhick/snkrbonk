# Sneaker Collection 👟

A mobile application for sneaker enthusiasts to catalogue and manage their sneaker collection with AI-powered image detection.

## Features

- **Add Sneakers** - Capture or upload photos of your sneakers with details
- **AI Detection** - Automatic sneaker recognition from images
- **View Collection** - Browse your complete sneaker catalogue
- **Update Details** - Edit sneaker information and images
- **Delete Items** - Remove sneakers from your collection

## Tech Stack

- **Frontend**: React Native with Expo
- **Authentication**: Clerk
- **Backend**: Convex
- **AI**: Image recognition for sneaker detection

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (v18 or higher)
- npm or yarn
- Expo CLI (`npm install -g expo-cli`)
- iOS Simulator (Mac) or Android Studio (for Android development)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/sneaker-collection.git
cd sneaker-collection
```

2. Install dependencies:
```bash
npm install
# or
yarn install
```

3. Set up environment variables:

Create a `.env` file in the root directory:
```env
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
EXPO_PUBLIC_CONVEX_URL=your_convex_deployment_url
```

4. Set up Convex:
```bash
npx convex dev
```

5. Start the development server:
```bash
npx expo start
```

## Configuration

### Clerk Authentication

1. Create a Clerk account at [clerk.com](https://clerk.com)
2. Create a new application
3. Copy your publishable key to the `.env` file
4. Configure OAuth providers (optional)

### Convex Backend

1. Sign up at [convex.dev](https://convex.dev)
2. Create a new project
3. Run `npx convex dev` to initialize
4. Deploy your functions with `npx convex deploy`

## Project Structure

```
├── app/                    # Application screens and navigation
├── components/             # Reusable React components
├── convex/                 # Convex backend functions and schema
├── assets/                 # Images, fonts, and other static files
├── hooks/                  # Custom React hooks
├── utils/                  # Utility functions and helpers
└── constants/              # App constants and configurations
```

## Usage

1. **Sign Up/Login**: Authenticate using Clerk
2. **Add a Sneaker**: Tap the '+' button, take a photo or upload from gallery
3. **AI Detection**: The app automatically detects sneaker details from the image
4. **View Collection**: Browse all your sneakers in a grid or list view
5. **Edit/Delete**: Long press on any sneaker to edit or remove it

## Development

### Running on iOS
```bash
npx expo start --ios
```

### Running on Android
```bash
npx expo start --android
```

### Running on Web
```bash
npx expo start --web
```

## Building for Production

### iOS
```bash
eas build --platform ios
```

### Android
```bash
eas build --platform android
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Expo](https://expo.dev) - React Native framework
- [Clerk](https://clerk.com) - Authentication platform
- [Convex](https://convex.dev) - Backend platform
- AI model providers for sneaker detection

## Support

For support, please open an issue in the GitHub repository or contact [your-email@example.com](mailto:fernanhick@gmail.com).

## Roadmap

- [ ] Barcode/QR code scanning
- [ ] Price tracking and market value
- [ ] Social sharing features
- [ ] Collection statistics and insights
- [ ] Dark mode support
- [ ] Export collection data
