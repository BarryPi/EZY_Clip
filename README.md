# EZY_Clip - Batch Export Clips to Audio Files
![Max for Live](https://img.shields.io/badge/Max%20for%20Live-8-orange)
![Ableton Live](https://img.shields.io/badge/Ableton%20Live-11%2B-blue)
![License](https://img.shields.io/badge/license-MIT-green)

A Max for Live device that simplifies exporting multiple audio clips from Ableton Live into individual audio files with intelligent naming and flexible formatting options.

![ezy-titleDef](https://github.com/user-attachments/assets/3c273c5e-3e94-4aa4-beb7-1553d063d2c1)


*Simple, fast, and flexible batch audio export for Ableton Live*

## Features

- **Batch Export**: Export all clips from a track in one click
- **Flexible Naming Modes**:
  - **Manual Mode**: Use your custom clip names from Ableton
  - **Automatic Mode**: Generate sequential names based on track name (e.g., Snare_01, Snare_02...)
- **Multiple Format Support**: 
  - AIFF, WAV
  - Mono/Stereo
  - 8-bit, 16-bit, 24-bit, 32-bit
- **Smart Validation**: 
  - Prevents exporting empty tracks
  - Warns before re-exporting same format
  - Clear status messages guide you through the process
- **Visual Progress Tracking**: Real-time progress bar and file-by-file export status
- **Drag & Drop Folder Selection**: Simply drop your destination folder to get started

## Demo

### Manual Naming Mode


### Automatic Naming Mode



## Requirements

- **Ableton Live**: 11 or higher
- **Max for Live**: 8 or higher
- **Operating System**: Windows / macOS

## Installation

1. Download `EZY_Clip.amxd` from the [Releases](../../releases) page
2. Place the file in your Ableton User Library:
   - **Windows**: `Documents\Ableton\User Library\Presets\Audio Effects\Max Audio Effect`
   - **Mac**: `~/Music/Ableton/User Library/Presets/Audio Effects/Max Audio Effect`
3. The device will appear in your **Max for Live** section under Audio Effects

## How to Use

### Basic Workflow

1. **Load the device** on any audio track in Ableton Live
2. **Drop a folder** into the "DROP YOUR FOLDER HERE" area - this is where your files will be saved
3. **Select a track** from the dropdown menu (tracks with sliced audio clips)
4. **Choose your export settings**:
   - File format (AIFF/WAV)
   - Channel mode (Mono/Stereo)
   - Bit depth (8/16/24/32-bit)
5. **Select naming mode**:
   - **A (Manual)**: Uses clip names from Ableton
   - **B (Auto)**: Uses track name with sequential numbering
6. **Click the export button** to start the process
7. Monitor progress in the status window and progress bar

### Important Notes

- ⚠️ **Select folder BEFORE choosing a track** for proper initialization
- The device will notify you if the selected track contains no clips
- You can re-export with different formats by changing settings and clicking export again
- Status messages guide you through each step of the process

## Interface Overview

**Left Panel**:
- 🔄 Reload button: Refresh track list if you've made changes to your Live set
- 📁 Folder drop zone: Drag and drop your destination folder
- 🎵 Track selector: Choose which track to export
- ⚙️ Format controls: Audio format, channels, and bit depth

**Right Panel**:
- 🔘 Export button: Start the export process
- 🔀 A/B toggle: Switch between Manual and Automatic naming modes
- 📊 Status window: Shows current operation and file paths
- 📈 Progress bar: Visual indication of export progress

## Use Cases

- **Sample Library Creation**: Quickly export sliced drum hits, vocal chops, or instrument samples
- **Stem Generation**: Export individual elements for mixing or collaboration
- **Sound Design**: Batch export variations of processed audio
- **Archive Projects**: Save individual clips before project cleanup
- **Quick Sharing**: Export specific clips to share with collaborators

## Technical Details

- Uses `sfrecord~` for high-quality audio rendering
- Validates track and clip data before processing
- Prevents accidental overwrites with format checking
- Real-time progress feedback during export

## Roadmap

Potential future features:
- Auto-open destination folder after export


## Support

If you encounter any issues or have feature requests, please [open an issue](../../issues) on GitHub.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

Created by [BarryPiasbian(PiNO)]

If you find this tool useful, enjoi it!!!

---

**Made with Max for Live** 🎛️
