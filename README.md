# TravelTip 🌎
> Your smart location manager

## Overview
TravelTip helps you track, manage and share your favorite locations with an intuitive map interface. Get real-time distance tracking, advanced filtering, and beautiful statistical visualizations.

## ✨ Core Features

### 📍 Location Management 
- Create locations via interactive map modal
- View detailed location info with distance tracking
- Edit location details seamlessly
- Delete with confirmation
- Smart filtering and dynamic sorting

### 🗺️ Map Integration
- Interactive Google Maps interface
- Address search & navigation
- User geolocation support
- Real-time distance calculations
- Smart map markers

### 📊 Analytics & Smart Features
- Rate distribution visualization
- Update status tracking (Today/Past/Never)
- Distance metrics when location enabled
- Advanced text filtering (name & address)
- Multi-parameter sorting
- URL-based state management
- Web Share API integration

## 🛠️ Technical Implementation

### Location Model
```js
{
    id: 'GEouN',
    name: 'Dahab, Egypt',
    rate: 5,
    geo: {
        address: 'Dahab, South Sinai, Egypt',
        lat: 28.5096676,
        lng: 34.5165187,
        zoom: 11
    },
    createdAt: 1706562160181,
    updatedAt: 1706562160181
}

Service Layer
jsCopyexport const locService = {
    query,
    getById,
    remove,
    save,
    setFilterBy,
    setSortBy,
    getLocCountByRateMap,
    getLocCountByUpdateMap
}

export const mapService = {
    initMap,
    getPosition,
    setMarker,
    panTo, 
    lookupAddressGeo,
    addClickListener
}
Controller Interface
jsCopywindow.app = {
    onRemoveLoc,
    onUpdateLoc, 
    onSelectLoc,
    onPanToUserPos,
    onSearchAddress,
    onCopyLoc,
    onShareLoc,
    onSetSortBy,
    onSetFilterBy
}
🚀 Setup Guide

Clone repository

bashCopygit clone https://github.com/shmuel-levy/TravelTip.git

Configure API key

jsCopyconst MAPS_API_KEY = 'your-api-key-here'

Enable Google APIs

Maps JavaScript API
Geocoding API


Launch

bashCopyopen index.html
