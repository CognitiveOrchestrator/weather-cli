# 🌤️ weather-cli

<div align="right">
<a href="README.md">中文版本</a>
</div>


[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Node.js](https://img.shields.io/badge/Node.js-20+-green.svg)](https://nodejs.org/)

A beautifully styled command-line weather query tool supporting Gaode Weather API and Open-Meteo.

## ✨ Features

| Feature | Command | Description |
|---------|---------|-------------|
| Multi-day Forecast | `--days 1-5` | 1-5 day weather forecast |
| Detailed Information | `--advanced` | Wind speed, update time, etc. |
| 24-hour Forecast | `--hourly` | Hour-by-hour weather changes |
| Air Quality | `--aqi` | AQI, PM2.5, PM10, etc. |
| JSON Output | `--json` | Suitable for script integration |
| Wallpaper Mode | `--wallpaper` | Clean, aesthetic card style |
| Unit Switch | `--unit` | Metric (°C) / Imperial (°F) |
| Local Cache | Automatic | 30-minute cache reduces API calls |

## 📦 Installation

### Global Installation

```bash
npm install -g .
```

### Local Usage

```bash
git clone https://github.com/CrazyMinions/weather-cli.git
cd weather-cli
npm install
```

## ⚙️ Configuration

Create a `.env` file in the project root:

```env
# Gaode Map Weather API Key (Required)
# Application URL: https://lbs.amap.com/
# Select "Web Service" type
GAODE_MAP_API_KEY=your_key_here

# Baidu Map API Key (Optional, for city resolution)
BAIDU_MAP_API_KEY=your_key_here
```

## 🚀 Usage

### Basic Usage

```bash
# Query Beijing weather
weather 北京

# Query Shanghai weather
weather 上海

# Use English city names
weather Beijing
weather Shanghai
```

## 🌍 Supported Cities

### Chinese Cities (100+)

Beijing, Shanghai, Guangzhou, Shenzhen, Chengdu, Hangzhou, Wuhan, Xi'an, Nanjing, Tianjin, Chongqing, Changsha, Kunming, Xiamen, Qingdao, Dalian, Shenyang, Harbin, Changchun, Zhengzhou, Jinan, Fuzhou, Hefei, Nanchang, Guiyang, Lanzhou, Yinchuan, Xining, Hohhot, Urumqi, Lhasa, Nanning, Haikou, Taipei, Hong Kong, Macau...

### International Cities

Tokyo, New York, London, Paris, Seoul, Singapore, Sydney, Los Angeles, San Francisco, Berlin, Moscow, Dubai, Bangkok, Mumbai, Toronto...

## 📊 Data Sources

| Data Type | Source | Notes |
|-----------|--------|-------|
| Chinese City Weather | Gaode Weather API | Real-time + 4-day forecast |
| International City Weather | Open-Meteo | Free, no API Key required |
| Air Quality | Open-Meteo Air Quality | Free, no API Key required |

## 🛠️ Development

```bash
# Install dependencies
npm install

# Run in development mode
npm run dev

# Build
npm run build

# Type checking
npm run typecheck
```

## 📄 License

MIT License

## 🤝 Contributing

Pull Requests are welcome!

## 🤖 About

This project was developed with assistance from OpenCode AI using the following models:

- **Primary Model**: SiliconFlow CN Pro/DeepSeek-V3.2
- **Model ID**: siliconflow-cn/Pro/deepseek-ai/DeepSeek-V3.2
- **AI Agent**: Sisyphus - OhMyOpenCode Senior Architect Agent

> 💡 This project demonstrates the complete workflow of AI-assisted development: requirements analysis, code implementation, testing, documentation, and continuous improvement.