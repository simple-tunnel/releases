# SimpleTunnel Releases

Official binary releases for SimpleTunnel - expose your local services to the internet with automatic HTTPS.

## Installation

### macOS/Linux via Homebrew

```bash
brew tap simple-tunnel/simpletunnel
brew install simpletunnel
```

### Manual Download

Download the appropriate binary for your platform from the [releases page](https://github.com/simple-tunnel/releases/releases).

- `simpletunnel-darwin-arm64` - macOS Apple Silicon (M1/M2)
- `simpletunnel-darwin-amd64` - macOS Intel
- `simpletunnel-linux-amd64` - Linux x86_64

Make it executable:
```bash
chmod +x simpletunnel-*
```

## Usage

```bash
# Basic usage
simpletunnel -port 8080

# Password protection
simpletunnel -port 8080 -password mypassword

# Custom domain
simpletunnel -port 8080 -domain example.com -root

# TCP tunneling
simpletunnel -port 22 -protocol tcp
```

## Documentation

Visit [simpletunnel.com](https://simpletunnel.com) for full documentation.

## License

SimpleTunnel is proprietary software. See LICENSE for details.