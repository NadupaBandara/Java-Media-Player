# 🎵 JavaFX Media Player

A basic media player built with **Java** and **JavaFX**, designed to play various types of audio files with a graphical interface.  
The project is modular and demonstrates **object-oriented principles**, the **Factory design pattern**, the **Iterator pattern**, and **JavaFX** for GUI development.

---

## 🚀 Features
- Play, pause, and stop audio files  
- WAV and tagged audio file support  
- Playlist management  
- Iterator pattern for looping through songs  
- JavaFX-based user interface  

---

## 🧱 Project Structure
The development process is split into five main parts:

### 1️⃣ Creating the `AudioFile` Class
This is the base abstract class that defines shared properties and methods for all types of audio files.  
It includes metadata such as file path and abstract methods for playing the file and retrieving information.

```java
public abstract class AudioFile {
    protected String filepath;

    public AudioFile(String filepath) {
        this.filepath = filepath;
    }

    public abstract void play();
    public abstract String getInfo();
}
