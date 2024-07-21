# Cat & Jess's Travel Planner

A simple React application for planning a trip with detailed itineraries.

## Features

- Display a day-by-day itinerary with activities and details.
- Toggle visibility of activity details for each day.
- Dynamic styling based on selected day and expanded items.

## Getting Started

### Prerequisites

Make sure you have the following installed on your development machine:

- [Node.js](https://nodejs.org/)
- [npm](https://www.npmjs.com/)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/username/travel-planner.git
   cd travel-planner
   ```

2. Install the dependencies:

   ```bash
   npm install
   ```

### Running the App

Start the development server:

```bash
npm start
```

Open [http://localhost:3000](http://localhost:3000) to view it in the browser. The page will reload if you make edits.

## Code Overview

### Main Components

- **TravelPlanner**: The main component that handles the itinerary display and state management.

### State Management

- `selectedDay`: Keeps track of the currently selected day in the itinerary.
- `expandedItems`: Manages the expanded state of each activity item to show or hide details.

### Functions

- `toggleItem(dayIndex, itemIndex)`: Toggles the visibility of details for a specific activity item.

### Itinerary Structure

The itinerary is defined as an array of objects, each representing a day with a date and a list of activities. Each activity has a time, a brief description (`activity`), and detailed information (`details`).

```jsx
const itinerary = [
  {
    date: 'Monday, July 8',
    items: [
      {
        time: '6:07 AM',
        activity: '✈️ Depart Ottawa (YOW) on WestJet Flight WS 611',
        details: 'Remember to arrive at the airport at least 2 hours early. Don\'t forget your travel documents!'
      },
      ...
    ],
  },
  ...
];
```

### Styling

Inline styles are used for simplicity, ensuring the app has a clean and functional user interface.

## Usage

1. **Day Selection**: Click on any date button to display the itinerary for that day.
2. **Toggle Activity Details**: Click on any activity to toggle the visibility of its detailed information.

## Customization

Feel free to modify the itinerary data and styles as needed. The current setup uses inline styles, but you can easily switch to a CSS-in-JS solution or an external stylesheet for more complex styling needs.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any improvements or bug fixes.

## License

This project is licensed under the MIT License.

## Acknowledgments

- React for providing a powerful library to build the UI.
- The creators of the itinerary content for providing detailed and structured trip information.

---

Happy travels, and enjoy planning your trip with Cat & Jess's Travel Planner!
