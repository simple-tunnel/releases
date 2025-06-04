# SimpleTunnel Releases

Official binary releases for SimpleTunnel - expose your local services to the internet with automatic HTTPS.

## 🚨 v2.0.0 Breaking Change

**Authentication Required**: Starting with v2.0.0, all users must obtain an API key from [simpletunnel.com](https://simpletunnel.com) to use SimpleTunnel.

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
# Set your API key (required!)
export SIMPLETUNNEL_API_KEY=st_live_your_key_here

# Basic usage
simpletunnel -port 8080

# Or pass key directly
simpletunnel -port 8080 -key st_live_your_key_here

# Password protection (Pro/Business only)
simpletunnel -port 8080 -password mypassword

# Custom domain
simpletunnel -port 8080 -domain example.com -root

# TCP tunneling (Pro/Business only)
simpletunnel -port 22 -protocol tcp
```

## Documentation

Visit [simpletunnel.com](https://simpletunnel.com) for full documentation.

## License

SimpleTunnel is proprietary software. See LICENSE for details.