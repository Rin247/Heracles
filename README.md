# Heracles — Offline Gym Coach with Procedural Figure Renderer

Heracles is a 100% offline, privacy-first Android workout coach and strength training tracker. Powered by a custom procedural forward-kinematics (FK) 2D anatomical figure renderer, Heracles visualizes real-time exercise biomechanics, active muscle group heatmaps, and movement joint angles without relying on pre-rendered video files or internet connections.

---

## 🏋️ Key Features & Subsystem Breakdown

### 🦾 Procedural FK Figure Renderer (`figure-render`)
- **Current**: 2D FK skeleton animation (`FkSkeleton`, `FkRenderer`), joint-angle keyframe interpolation, muscle group engagement heatmap, and 60 FPS Canvas rendering.
- **Planned / Roadmap**: 3D mesh anatomical figure option, custom exercise pose recorder, and biomechanical stress vector overlays.

### 📝 Workout Logger & Routine Builder (`workout-log`)
- **Current**: Custom routine creator, set/rep/weight logging, rest timer countdown, RPE tracking, and 1RM (One Rep Max) calculator.
- **Planned / Roadmap**: Automated progressive overload recommendations, superset/drop-set grouping, and plate math visualizer.

### 📊 Muscle Recovery & Volume Analytics (`analytics`)
- **Current**: Muscle fatigue heatmap, weekly volume charts per muscle group, and strength progression trends.
- **Planned / Roadmap**: Deload cycle predictor, body measurement tracker, and exercise substitution recommender.

---

## 🏗️ Architecture & Technology Stack

- **Platform**: Android 13+ (minSdk 33, targetSdk 37).
- **UI & Graphics**: Kotlin, Jetpack Compose, Canvas FK Gait Engine.
- **Database**: Room local database.
- **Licensing**: AGPL-3.0.

---

## 🛠️ Building & Running

```bash
./gradlew assembleDebug
./gradlew installDebug
```

---

## 📜 License

Heracles is released under the **GNU Affero General Public License v3.0** (AGPL-3.0). See [`LICENSE`](LICENSE) for details.
