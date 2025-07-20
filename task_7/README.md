# Ecommerce Mobile App

A simple ecommerce mobile app built with Flutter that allows users to create, view, update, and delete products.

## Features

- **Home Screen**: Displays a list of all products with a clean card-based layout
- **Add Product**: Form to create new products with title, description, and price
- **Edit Product**: Update existing product information
- **Product Details**: View detailed information about a specific product
- **Delete Product**: Remove products with confirmation dialog
- **Smooth Animations**: Enhanced user experience with navigation transitions
- **Named Routes**: Organized navigation structure
- **Data Passing**: Seamless data flow between screens

## Screens

### 1. Home Screen (`/`)
- Displays all products in a scrollable list
- Empty state when no products exist
- Floating action button to add new products
- Tap on any product to view details

### 2. Add/Edit Product Screen (`/add-product`, `/edit-product`)
- Form with validation for product title, description, and price
- Different titles and behaviors for add vs edit mode
- Smooth slide-in animation
- Cancel and save options

### 3. Product Detail Screen (`/product-detail`)
- Full product information display
- Edit and delete actions via menu
- Confirmation dialog for deletion
- Scale and fade animations

## Navigation Features

- **Named Routes**: All screens use named routes for better organization
- **Data Passing**: Products are passed between screens using route arguments
- **Back Button Handling**: Proper navigation stack management
- **Smooth Animations**: Custom animations for better user experience
- **Result Handling**: Screens return results to update the product list

## Getting Started

### Prerequisites
- Flutter SDK (>=2.17.0)
- Dart SDK
- Android Studio or VS Code with Flutter extensions

### Installation

1. Clone the repository:
\`\`\`bash
git clone <repository-url>
cd ecommerce_app
\`\`\`

2. Install dependencies:
\`\`\`bash
flutter pub get
\`\`\`

3. Run the app:
\`\`\`bash
flutter run
\`\`\`

## Project Structure

\`\`\`
lib/
├── main.dart                 # App entry point and route configuration
├── models/
│   └── product.dart         # Product data model
└── screens/
    ├── home_screen.dart     # Product list screen
    ├── add_edit_product_screen.dart  # Add/Edit product form
    └── product_detail_screen.dart    # Product details view
\`\`\`

## Technical Implementation

### Navigation
- Uses Flutter's built-in `Navigator` with named routes
- Route arguments for passing data between screens
- Proper back button handling and navigation stack management

### Animations
- `AnimationController` with `TickerProviderStateMixin`
- Fade, slide, and scale transitions
- Smooth 300-400ms duration animations

### State Management
- `StatefulWidget` with `setState()` for local state
- Data flows through constructor parameters and route arguments
- Proper disposal of controllers and animations

### UI/UX
- Material Design components
- Consistent color scheme and typography
- Responsive layout with proper spacing
- Form validation and error handling
- Loading states and empty states

## Code Quality

- Clean, readable code structure
- Proper widget composition
- Resource disposal (controllers, animations)
- Form validation
- Error handling
- Consistent naming conventions

## Future Enhancements

- Add image upload functionality
- Implement local storage (SQLite/Hive)
- Add search and filter capabilities
- Implement categories
- Add shopping cart functionality
- User authentication
- API integration
