Modular Media Streaming Suite (Java)

This project showcases a modular media streaming system built in Java, highlighting the usage of several structural design patterns. Playback behavior is simulated through console output, demonstrating how these patterns contribute to building an extensible and maintainable media player architecture.



Structural Patterns Used

- **Bridge** — Decouples the media player’s abstraction from its rendering implementations (software vs. hardware).
- **Adapter** — Enables compatibility with older or incompatible media sources.
- **Decorator** — Allows optional runtime enhancements such as watermarks and equalizer settings without modifying core logic.
- **Composite** — Provides support for standard and nested playlists, enabling hierarchical media organization.
- **Proxy** — Caches remote streams to improve performance during repeated access.



Core Capabilities

- Playback of media from:
  - Local files
  - Remote APIs
  - HLS live streams
- Nested playlist handling via the Composite pattern
- Runtime switching between CPU and GPU renderers
- Add-on audio/visual effects through decorators
- Remote media caching for improved loading times
- Legacy media support through adapters



Setup & Usage

Requirements
- **Java 17 or newer** (built and tested on JDK 25)
- Visual Studio Code with the **Java Extension Pack**, or any Java-compatible IDE



 Running in VS Code

1. Open the project folder in **Visual Studio Code**.
2. Install the **Java Extension Pack** if prompted.
3. Open **`Demo.java`**.
4. Run using the configuration **"Run Modular Media Suite"** or press **Ctrl + F5**.

---
 Running from the Command Line

From the root directory of this repository, execute:

mkdir -p out
javac -d out $(find src/main/java -name "*.java")
java -cp out com.example.media.Demo
