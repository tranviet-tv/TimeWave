# TimeWeave - Meeting Scheduler Features

TimeWeave is an advanced, web-based meeting scheduling tool designed to effortlessly find the best meeting times for groups of people. By intelligently aggregating participants' availability and handling complex timezone conversions, it takes the hassle out of scheduling. 

Here is a comprehensive breakdown of all the features available in this project:

## 🌟 Core Capabilities

- **Lightning Fast Scheduling**: Designed to handle meetings for medium-to-large groups (5 to 50 people) and calculate the optimal times in under 500ms.
- **Smart Timezone Handling**: Completely eliminates timezone confusion. The system automatically converts and normalizes all times to UTC on the backend, allowing users from anywhere in the world to view and select times in their local timezone.
- **Interactive Heatmap Display**: Visualizes group availability using an intuitive color-coded heatmap. The darker the green color on a timeslot, the more people are available to meet at that specific time.
- **AI-Powered Setup (Google Gemini)**: 
  - *For Leaders*: Allows the meeting organizer to create a meeting simply by typing a natural language prompt (e.g., "Schedule a 45-minute sync next week with the marketing team").
  - *For Participants*: Allows attendees to input their busy times using natural language instead of manually clicking on a calendar.

## 🧑‍💼 For Meeting Organizers (Leaders)

- **3-Step Setup Wizard**: A streamlined, intuitive flow for creating a meeting request:
  1. **Configuration**: Define the meeting title, description, duration (15 to 480 minutes), date range, and default timezone.
  2. **Invites**: Add participants manually, import them in bulk, or generate a public link to share on your own.
  3. **Confirmation**: Preview the blank heatmap and dispatch invitations.
- **Real-Time Progress Tracking**: The dashboard provides a progress bar showing the percentage of invitees who have responded.
- **Automated "Top Suggestions"**: The system automatically ranks and suggests the best timeslots based on the highest number of available participants.
- **Finalizing and Chốt Lịch**: Once the organizer decides on a time, they can "finalize" the meeting with a single click.

## 👥 For Participants (Members)

- **Frictionless Entry**: Participants can access the scheduling link without needing to create an account. They only need to provide their name and (optionally) their email.
- **Drag-and-Drop Calendar**: An easy-to-use visual calendar where participants can click and drag to paint over the blocks of time they are "busy".
- **Live Updates**: As soon as a participant saves their availability, the group heatmap is immediately updated.

## ✉️ Email & Notifications System

- **Email Verification**: Ensures security and authenticity by validating user emails before allowing certain administrative actions.
- **Automated Invitations**: The system can automatically dispatch beautifully formatted email invitations to all participants containing their unique response link.
- **Finalized Notifications**: Once the organizer selects the winning timeslot, the system automatically blasts an email to all participants with the final meeting time and details.
- *Powered by Resend API for reliable delivery.*

## 🔒 Security & Architecture

- **Role-based Workflows**: Clear separation of permissions between the meeting organizer (who has the admin token to finalize) and the participants (who can only submit their times).
- **Responsive Web Design**: Built with Bootstrap 5, ensuring the app works perfectly on desktops, tablets, and mobile devices.

## 🚀 Upcoming Features (Roadmap)
- Export to `.ics` calendar files.
- Direct OAuth integration with Google Calendar and Outlook Calendar.
- Real-time updates via WebSockets.
- Multi-language localization support.
