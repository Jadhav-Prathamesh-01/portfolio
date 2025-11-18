# Portfolio Jenkins Setup

## Quick Start Commands

### 1. Clone Repository
```bash
git clone https://github.com/Jadhav-Prathamesh-01/portfolio.git
cd portfolio
```

### 2. Install and Start Jenkins
```bash
# Install Jenkins
brew install jenkins-lts

# Start Jenkins
brew services start jenkins-lts

# Get initial admin password
cat ~/.jenkins/secrets/initialAdminPassword
```

### 3. Access Jenkins
```bash
# Open Jenkins in browser
open http://localhost:8080
```

### 4. Push Changes to Trigger Build
```bash
# Add changes
git add .

# Commit changes
git commit -m "your commit message"

# Push to GitHub (triggers Jenkins build)
git push origin main
```

### 5. Access Deployed Website
```bash
# Website runs on
http://localhost:3000
```

### Stop Services
```bash
# Stop Jenkins
brew services stop jenkins-lts

# Stop local server
pkill -f "python3 -m http.server 3000"
```