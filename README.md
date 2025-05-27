# SpeechLogix_SDK
🧾 Project Role: GIS-Integrated VoIP Region Validator for Flutter App
You are building a geofencing-based VoIP calling system where users can make or receive calls only within their assigned telecom region, based on geographic boundaries (districts, taluks) in Kerala and Lakshadweep.

Your responsibilities include:

🧠 1. GIS-Based Region Mapping
Working with shapefiles of Indian districts (especially Kerala) and Lakshadweep.

Using QGIS to:

Load, view, and edit district and taluk boundaries.

Merge districts/taluks into Business Areas (BA) like "Ernakulam BA", "Kozhikode BA".

Assign BA Codes (like EK, KKD, etc.) and STD codes (like 0484, 0495, etc.) as attributes.

Export GIS boundaries to usable formats like GeoJSON, Shapefile, or GeoPackage for app integration.

📍 2. Geolocation-Based Decision Logic
Building logic to:

Fetch a user’s live location in a Flutter app.

Check if the location falls within the polygon boundary of their Caller ID's (CID) assigned BA.

Enable calling and receiving if the user is inside the district; allow receiving only if outside.

📦 3. Flutter Package Development
Designing a reusable Flutter plugin/package that:

Integrates GPS, polygon-based geofencing, and CID-based access control.

Validates location-to-BA mapping in real time.

Ensures the caller’s CID prefix matches their current district location polygon.

🛠️ Tools & Technologies Used
QGIS (for polygon editing and spatial data processing)

GeoJSON/Shapefiles (for boundary data)

Flutter/Dart (for mobile app development)

Location/GPS packages (to fetch real-time user coordinates)

Custom VoIP logic (for call permissions based on location)

