# Intune Log Reader for Windows

## Overview

Intune Log Reader provides real-time analysis and monitoring of Microsoft Intune Management Extension logs on Windows systems.

⚠️ Warning: Unauthorized forks of this repository may contain malicious code. Always download from this official repo only: https://github.com/pathaksomesh06/Intune-Log-Reader-for-Windows

## Features

- **Automated Log Parsing**: Processes Windows Intune log format automatically
- **Smart Categorization**: Organizes logs into Device, Applications, Configurations, Compliance, Sync Status
- **Error Pattern Detection**: Identifies recurring error patterns and frequency
- **Professional Dashboard**: Real-time statistics and category breakdown
- **Advanced Search**: Filter by log level, component, timestamp, message content
- **Export Functions**: CSV export and detailed report generation
- **Live Monitoring**: Real-time log updates (when available)

## Screenshots
<img width="1267" height="711" alt="Screenshot 2025-09-14 at 00 00 34" src="https://github.com/user-attachments/assets/d481fe3a-35c3-4245-be4d-aebbe1c1cbc6" />
<img width="993" height="556" alt="Screenshot 2025-09-14 at 00 03 03" src="https://github.com/user-attachments/assets/817a2392-4f89-4e3a-b1b1-0711989cd938" />
<img width="1265" height="709" alt="Screenshot 2025-09-14 at 00 03 30" src="https://github.com/user-attachments/assets/f93d346a-c29a-4fd0-b668-e9a9b1b353a4" />
<img width="1264" height="712" alt="Screenshot 2025-09-14 at 00 03 49" src="https://github.com/user-attachments/assets/881135cd-a1ca-4c8a-89bb-f36aa2ae1fe0" />
<img width="1264" height="710" alt="Screenshot 2025-09-14 at 00 04 16" src="https://github.com/user-attachments/assets/b3acde62-114b-4f7f-b789-716e857f4f28" />
<img width="1267" height="711" alt="Screenshot 2025-09-14 at 00 04 43" src="https://github.com/user-attachments/assets/67f900a3-ccb8-46c5-b8bd-5c4d2c60aa61" />
<img width="1259" height="705" alt="Screenshot 2025-09-14 at 00 05 26" src="https://github.com/user-attachments/assets/8abbad80-4c86-4182-8811-fc6c597db32b" />
<img width="1262" height="708" alt="Screenshot 2025-09-14 at 00 05 44" src="https://github.com/user-attachments/assets/1f03618f-0dcd-485e-8b60-b26393e99f74" />


## Installation

### Method 1: Windows Installer (Recommended)
1. Download `IntuneLogReader_Setup_v1.0.exe` from releases
2. Run installer with administrator privileges
3. Follow installation wizard
4. Launch from Desktop shortcut or Start Menu

### Method 2: Portable Version
1. Download and extract release ZIP
2. Navigate to `release` folder
3. Run `intune_log_reader_windows.exe`

## Log Sources

Automatically loads from: `C:\ProgramData\Microsoft\IntuneManagementExtension\Logs`

Supported log files:
- AgentExecutor.log
- AppActionProcessor.log
- AppWorkload.log
- DeviceHealthMonitoring.log
- HealthScripts.log
- IntuneManagementExtension.log

## Usage

1. **Launch Application**: Start from Desktop or Start Menu
2. **Load Logs**: Click refresh icon to auto-load all Intune logs
3. **Navigate Categories**: Use sidebar to filter by log category
4. **Analyze Errors**: Review Top Error Patterns on Dashboard
5. **Export Data**: Use Export menu for CSV or detailed reports
6. **Search Logs**: Use search bar within each category

## Technical Stack

- **Framework**: Flutter 3.35.3
- **Language**: Dart 3.9.2
- **Platform**: Windows Desktop
- **Build**: Release optimized

### Build Commands
```bash
flutter pub get
flutter build windows --release
```

### Project Structure
```
lib/
├── models/           # Data models (LogEntry, LogCategory)
├── services/         # Core services (LogFileService, LogCategorizationService)
├── views/           # UI components (CategoryView)
└── main.dart        # Application entry point
```

### Future Roadmap

#### Version 1.1 (Planned)
- Custom log path configuration
- Trend analysis charts
- Advanced search operators

#### Version 1.2 (Planned)
- Multi-language support
- Theme customization
- Plugin architecture
- Scheduled exports

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**Somesh Pathak**
- GitHub: [@pathaksomesh06](https://github.com/pathaksomesh06)
