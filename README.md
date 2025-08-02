# Airbnb Clone

A full-stack web application that replicates core features of Airbnb, allowing users to list, discover, and book accommodations.
## Overview

This project is a simplified Airbnb-like web application built with Node.js, Express, and EJS templating. Users can browse, add, edit, and delete home listings, mark homes as favourites, and view bookings. Data is stored in JSON files, and Tailwind CSS is used for styling.

## Project Structure

```
Airbnb/
├── app.js
├── package.json
├── nodemon.json
├── tailwind.config.js
├── controllers/
│   ├── errors.js
│   ├── hostController.js
│   └── storeController.js
├── data/
│   ├── favourite.json
│   └── homes.json
├── models/
│   ├── favourite.js
│   └── home.js
├── public/
│   ├── home.css
│   ├── output.css
│   └── images/
├── routes/
│   ├── hostRouter.js
│   └── storeRouter.js
├── utils/
│   └── pathUtil.js
└── views/
    ├── 404.ejs
    ├── host/
    ├── partials/
    ├── store/
    └── input.css
```

## Usage

- **Home Page:** View all available homes.
- **Homes List:** `/homes` — See all registered homes.
- **Favourites:** `/favourites` — View and manage your favourite homes.
- **Bookings:** `/bookings` — View bookings (static page).
- **Host Homes:** `/host/host-home-list` — Manage your hosted homes.
- **Add Home:** `/host/add-home` — Add a new home listing.

## Data Storage

- Home and favourite data are stored as JSON files in the `data/` directory.
- No external database is required.

## Customization

- **Styling:** Modify `input.css` and rebuild Tailwind CSS to update styles.
- **Images:** Add home images to `public/images/`.

## License

This project is for educational purposes.
## Features

- User authentication (sign up, login, logout)
- List properties with images, descriptions, and pricing
- Search and filter listings by location, date, and price
- Book and manage reservations
- User profile management
- Responsive design for mobile and desktop

## Tech Stack

- **Frontend:** EJS templating, Tailwind CSS
- **Backend:** Node.js, Express.js

## Getting Started

### Prerequisites

- Node.js & npm
- MongoDB instance (local or cloud)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/mujahidul885/Airbnb-nodejs-clone.git
    cd airbnb-clone
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Run Tailwind CSS build (if you want to update styles):
    ```
    npx tailwindcss -i ./views/input.css -o ./public/output.css --watch
    ```

4. Start the development server:
    ```bash
    npm start
    ```
5. Open your browser and visit:
   ```bash
   http://localhost:3000
   ```

## Folder Structure

```
/client      # EJS templates frontend
/server      # Node.js backend
/README.md   # Project documentation
```

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

[MIT](LICENSE)
