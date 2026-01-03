# Meetup Events

A modern React-based meetup events platform where users can discover, browse, and explore various events. The application features event filtering, search functionality, and detailed event information including speakers, schedules, and venue details.

---

## Demo Link

[Live Demo](
meetup-frontend-peach.vercel.app )

---

## Quick Start

```bash
git clone https://github.com/r60235/Meetup-Events.git
cd meetup-events
npm install
npm run dev
```

## Technologies

- **Frontend Framework:** React 19.1.1
- **Routing:** React Router DOM 7.9.3
- **Styling:** Bootstrap 5.3.8
- **Build Tool:** Vite 7.1.7


## Demo Video

Watch a walkthrough (5–7 minutes) of all major features of this app:
[Video Link](https://drive.google.com/file/d/1SfrCFuXgTfi1kyPpr7QKLAYHEPVMpL4k/view?usp=drive_link)

## Features

**Event Discovery**
- Browse all available meetup events with responsive card layout
- Filter events by type (Online/Offline)
- Real-time search functionality by event title and tags
- Visual indicators for event types (Online: green badge, Offline: red badge)

**Event Listings**
- Clean, modern card-based event display
- Event images with overlay type indicators
- Quick access to event date, time, and title information
- Seamless navigation to detailed event pages

**Event Details**
- Comprehensive event information including description and additional details
- Event scheduling with start/end times and dates
- Venue information and address details
- Ticket pricing information (Free or paid events)
- Speaker profiles with images, names, and roles
- Event tags for easy categorization
- Dress code and age restriction information

**Search & Filter**
- Dynamic search across event titles and tags
- Event type filtering (All, Online, Offline)
- Instant results with no page refresh required

**Responsive Design**
- Mobile-first responsive layout
- Bootstrap-powered UI components
- Optimized for all screen sizes

## API Reference

### **GET /events**
List all available meetup events

**Sample Response:**
```json
[
  {
    "_id": "event123",
    "title": "React Developers Meetup",
    "type": "Online",
    "startDate": "2024-02-15",
    "startTime": "18:00",
    "endTime": "20:00",
    "imgUrl": "https://example.com/event-image.jpg",
    "eventTags": ["React", "JavaScript", "Frontend"]
  }
]
```

### **GET /event/:id**
Get detailed information for a specific event

**Sample Response:**
```json
{
  "_id": "event123",
  "title": "React Developers Meetup",
  "type": "Online",
  "startDate": "2024-02-15",
  "startTime": "18:00",
  "endTime": "20:00",
  "hostedBy": "Tech Community Leaders",
  "eventImgUrl": "https://example.com/detailed-image.jpg",
  "details": "Join us for an exciting discussion about React best practices...",
  "eventAddress": "Virtual Event - Zoom Link Provided",
  "eventTicketPrice": 0,
  "eventTags": ["React", "JavaScript", "Frontend"],
  "speakerDetails": [
    {
      "name": "John Doe",
      "role": "Senior React Developer",
      "imgUrl": "https://example.com/speaker.jpg"
    }
  ],
  "additionalInfo": {
    "dressCode": "Casual",
    "ageRestriction": "18+"
  }
}
```

## Custom Hooks

**useFetch Hook**
- Handles API requests with loading and error states
- Provides clean data fetching interface
- Automatic loading state management

## Development Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
```

## Environment Setup

The application connects to a backend API hosted at:
`https://meetup-backend-silk.vercel.app`

For local development, ensure the backend service is running or update the API endpoints in the components.



## Contact

For bugs, feature requests, or questions, please reach out to:
- Email: rishaabh105@gmail.com

