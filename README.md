# 🔒 VaultX - Secure Password Manager

A modern, professional password manager built with Python and PyQt5, featuring strong encryption and a beautiful user interface.

![VaultX Logo](assets/splash.png)

## ✨ Features

- **🔐 Strong Encryption**: Uses Argon2 for password hashing and Fernet for data encryption
- **🎨 Modern UI**: Professional dark/light theme with custom SpaceX font
- **🔑 Password Generator**: Generate secure passwords with customizable criteria
- **📱 Responsive Design**: Clean, intuitive interface optimized for productivity
- **🔍 Search Functionality**: Quickly find passwords by app name or username
- **📋 Copy to Clipboard**: One-click password copying with visual feedback
- **👁️ Show/Hide Passwords**: Toggle password visibility with eye icon
- **💾 Local Storage**: All data encrypted and stored locally on your device

## 🚀 Installation

### Prerequisites
- Python 3.8 or higher
- pip package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/vaultx.git
   cd vaultx
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   - Windows:
     ```bash
     venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
   ```bash
   pip install -r requirement.txt
   ```

5. **Run the application**
   ```bash
   python main.py
   ```

## 🛡️ Security Features

### Encryption
- **Master Password**: Secured with Argon2 (industry-standard password hashing)
- **Vault Data**: Encrypted using Fernet (AES-128 in CBC mode)
- **Salt Generation**: Unique salt for each installation
- **Key Derivation**: PBKDF2 with 100,000 iterations

### Data Protection
- All sensitive data is encrypted before storage
- No data is transmitted over the network
- Local storage only - your data stays on your device
- Secure memory handling with automatic cleanup

## 🎨 User Interface

### Design Philosophy
- **Minimalist**: Clean, distraction-free interface
- **Accessible**: High contrast and readable typography
- **Responsive**: Adapts to different screen sizes
- **Professional**: Modern design suitable for business use

### Custom Branding
- **SpaceX Font**: Custom typography for a unique look
- **Color Palette**: Professional indigo-based color scheme
- **Icons**: Modern emoji-based icons for better accessibility
- **Animations**: Smooth transitions and hover effects

## 📁 Project Structure

```
VaultX/
├── main.py                 # Application entry point
├── requirement.txt         # Python dependencies
├── README.md              # This file
├── assets/                # Static assets
│   ├── fonts/            # Custom fonts
│   ├── icons/            # Application icons
│   └── splash.png        # Splash screen
├── core/                  # Core functionality
│   └── crypto.py         # Encryption and security
├── ui/                    # User interface
│   ├── login.py          # Login screen
│   ├── dashboard.py      # Main dashboard
│   ├── add_password.py   # Add password form
│   └── password_generator.py # Password generator
├── utils/                 # Utilities
│   ├── branding.py       # Branding and styling
│   ├── theme_manager.py  # Theme management
│   └── favicon_fetcher.py # Website icon fetching
└── vault/                 # Encrypted data storage
    ├── vault.json.enc    # Encrypted password data
    ├── salt.bin          # Encryption salt
    └── master.hash       # Master password hash
```

## 🔧 Configuration

### Customization Options
- **Theme**: Toggle between dark and light themes
- **Font Size**: Adjustable through system settings
- **Window Size**: Resizable main window
- **Password Criteria**: Customizable password generation rules

### Security Settings
- **Master Password**: Set once during first launch
- **Auto-lock**: Configure session timeout
- **Backup**: Export encrypted vault data

## 🚀 Usage

### First Launch
1. Launch the application
2. Set your master password (minimum 8 characters)
3. Start adding your passwords

### Adding Passwords
1. Click "Add Password" in the sidebar
2. Fill in the application name, username, and password
3. Optionally add a URL for favicon fetching
4. Click "Save" to encrypt and store

### Password Generator
1. Navigate to "Generator" in the sidebar
2. Configure password criteria (length, character types)
3. Click "Generate" to create a secure password
4. Use "Copy" to copy to clipboard

### Managing Passwords
- **Search**: Use the search bar to find specific passwords
- **Show/Hide**: Click the eye icon to toggle password visibility
- **Copy**: Click the clipboard icon to copy passwords
- **Edit**: Click "Edit" to modify password details
- **Delete**: Click "Delete" to remove passwords

## 🛠️ Development

### Building from Source
```bash
# Install development dependencies
pip install -r requirement.txt

# Run in development mode
python main.py

# Create executable (Windows)
pyinstaller --onefile --windowed main.py
```

### Code Style
- Follow PEP 8 guidelines
- Use type hints where appropriate
- Document all public methods
- Maintain consistent naming conventions

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Test all changes thoroughly
- Update documentation as needed
- Follow the existing code style
- Add appropriate error handling

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **PyQt5**: For the robust GUI framework
- **Cryptography**: For secure encryption algorithms
- **Argon2**: For secure password hashing
- **SpaceX Font**: For the custom typography

## 📞 Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/anuragaman25/VaultX/issues) page
2. Create a new issue with detailed information
3. Include your operating system and Python version

## 🔮 Roadmap

### Planned Features
- [ ] Password strength analyzer
- [ ] Secure notes storage
- [ ] Password sharing (encrypted)
- [ ] Browser extension integration
- [ ] Cloud backup (optional)
- [ ] Two-factor authentication
- [ ] Password expiration reminders
- [ ] Import/export functionality

### Performance Improvements
- [ ] Optimize large vault performance
- [ ] Reduce memory usage
- [ ] Faster search algorithms
- [ ] Improved UI responsiveness

---

**VaultX** - Your secure password companion 🔒
