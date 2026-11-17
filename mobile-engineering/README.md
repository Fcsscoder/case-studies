# Mobile Engineering Case Studies

This category highlights mobile application development with React Native and Expo, focusing on cross-platform performance, battery-efficient real-time transit timelines, accessible animation design, regulatory privacy compliance, and Android native alarm integrations.

---

## Case Studies in this Track

### 1. [Real-Time Fleet Transit Navigation & Privacy-Preserving Mobile Application](campus-mobility-transit-app/README.md)
* **Core Themes:** React Native, Expo, Geolocation & Transit, Accessibility, Regulatory Privacy Gates.
* **Key Challenges:**
  - Designing a single-stroke animated bus timeline with an accessible pulsating origin that dynamically collapses under OS-level `prefers-reduced-motion` settings.
  - Enforcing a strict technical privacy gate that prevents any network telemetry or background queries from executing prior to explicit user terms acceptance.
  - Scheduling exact departure reminder notifications using Android's native `SCHEDULE_EXACT_ALARM` permissions.
* **Technologies:** React Native, Expo, TypeScript, NativeWind (Tailwind CSS), Android Native Bridge, Jest.
