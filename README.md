﻿# 02230306-WEB101-PA2

# Pokedex Webpage Using React

## Introduction
This Pokedex webpage is developed using the React framework. It serves as a comprehensive resource for Pokemon enthusiasts, allowing them to search for and retrieve detailed information about their favorite Pokemon, as well as keep track of the Pokemon they have "caught." The project leverages React's component-based architecture, state management with Zustand, and API integration to create a fully functional and interactive Pokedex.

## Requirements
- **Search Feature**: Users can search for Pokemon by name or other relevant criteria using the official PokeAPI.
- **Display Pokemon Details**: Upon searching, relevant details of the searched Pokemon, such as name, type, abilities, stats, and an image, are displayed.
- **Catch Pokemon**: Users can "catch" Pokemon and maintain a list of caught Pokemon using Zustand for state management.
- **Component-Based Architecture**: The application is built using React's component-based architecture for modularity, maintainability, and reusability.
- **UI Component Library**: The project uses the `shadcn/ui` component library for building the user interface.

## Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Baluthegoat/02230306-WEB101-PA2
   cd pokedex

2. ## Installation 
   ```bash
   bun install
3. ## Start the development server
   ```bash
   bun run dev

## Usage
Open your browser and go to http://localhost:3000.

Use the search bar to find a specific Pokemon by name.

View detailed information about the Pokemon in the displayed results.

Click the "Catch" button to add the Pokemon to your list of caught Pokemon.

View your list of caught Pokemon in the "Caught Pokemon" section.

## Features
Search for Pokemon: Utilize the search feature to find Pokemon by name.

View Pokemon Details: See detailed information about the Pokemon, including their type, abilities, stats, and image.

Catch Pokemon: Keep track of the Pokemon you've caught using Zustand for state management.

## Technologies Used
React: A JavaScript library for building user interfaces.

Fetch API: For making API calls to the PokeAPI.

Zustand: For state management.

shadcn/ui: UI component library used for building the user interface.

PokeAPI: The API used to fetch Pokemon data.

## Detailed Component Description

1. SearchBar.js
Handles the search functionality. It includes an input field for the user to type the name of the Pokemon and a button to trigger the search.

2. PokemonCard.js
Displays the detailed information of a single Pokemon. This component receives the Pokemon data as props and renders the name, type, abilities, stats, and image.

3. PokemonList.js
Manages the list of Pokemon results from the search. It maps through the search results and renders a PokemonCard for each Pokemon.

4. CaughtPokemonList.js
Displays the list of Pokemon that the user has "caught." This component uses Zustand to manage and access the state of caught Pokemon.

5. usePokemonData.js
A custom hook that handles the API calls to fetch Pokemon data. It uses the Fetch API to request data from the PokeAPI.

6. usePokemonStore.js
Contains the Zustand store logic for managing the state of caught Pokemon. It includes actions for adding and removing Pokemon from the caught list.
