# AI Advertisement Generator 🎯

A modern web application that generates professional advertisements using Google's Gemini AI. Built with Next.js, TypeScript, and Tailwind CSS.

![AI Ad Generator](https://img.shields.io/badge/Next.js-14.0-black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.3-38B2AC)

## Features ✨

- 🤖 AI-powered advertisement generation using Google Gemini
- 🌍 Multi-language support (English & Arabic)
- 🎨 Modern, responsive UI with Tailwind CSS
- ⚡ Fast performance with Next.js
- 📱 Mobile-friendly design
- 🎯 Customizable tone and audience targeting

## Prerequisites 📋

- Node.js 16+ and npm/yarn
- Google Gemini API key (free at [makersuite.google.com](https://makersuite.google.com/app/apikey))

## Installation 🚀

### 1. Clone the Repository
```bash
git clone https://github.com/ashraflx71/ai_ad_generator.git
cd ai_ad_generator
```

### 2. Extract the ZIP File (if needed)
```bash
unzip ai-ad-generator.zip
```

### 3. Install Dependencies
```bash
npm install
```

### 4. Configure Environment Variables
Create a `.env.local` file in the root directory:

```bash
# Copy from example
cp .env.local.example .env.local

# Edit .env.local and add your Gemini API key
NEXT_PUBLIC_GEMINI_API_KEY=your_api_key_here
```

Get your API key:
1. Go to [https://makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey)
2. Click "Create API Key"
3. Copy and paste it into `.env.local`

### 5. Run Development Server
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Usage 💡

1. **Enter Product/Service**: Describe what you're advertising
2. **Specify Target Audience**: Who do you want to reach?
3. **Choose Tone**: Select professional, casual, humorous, or formal
4. **Generate**: Click "Generate Ad" to create the advertisement
5. **Copy**: Use the copy button to save the generated ad

## Available Scripts 📝

```bash
# Development
npm run dev

# Production build
npm run build

# Start production server
npm start

# Linting
npm run lint
```

## Project Structure 📁

```
ai-ad-generator/
├── app/
│   ├── globals.css          # Global styles
│   ├── layout.tsx           # Root layout
│   └── page.tsx             # Home page
├── components/
│   ├── AdGenerator.tsx      # Main generator component
│   ├── LanguageContext.tsx  # Language state management
│   ├── LanguageToggle.tsx   # Language switcher
│   └── Disclaimer.tsx       # Disclaimer component
├── lib/
│   └── gemini.ts            # Gemini API integration
├── .env.local.example       # Environment variables template
├── tsconfig.json            # TypeScript configuration
├── tailwind.config.ts       # Tailwind configuration
└── package.json             # Dependencies
```

## Technologies Used 🛠️

- **Next.js 14**: React framework
- **TypeScript**: Type safety
- **Tailwind CSS**: Styling
- **Google Generative AI**: AI capabilities
- **PostCSS**: CSS processing

## Troubleshooting 🔧

### "API key is not configured"
- Make sure `.env.local` exists
- Verify `NEXT_PUBLIC_GEMINI_API_KEY` is set correctly
- API key must start with the correct format

### "Cannot find module"
```bash
rm -rf node_modules
npm install
```

### Port 3000 is already in use
```bash
npm run dev -- -p 3001
```

### TypeScript errors
```bash
npm run build
# Check for errors in the output
```

## Performance Tips ⚡

- Ads generate in 2-5 seconds depending on internet speed
- Responses are cached for 60 seconds
- Use different tones for variety

## Security Note 🔒

- API key is public (NEXT_PUBLIC_) for browser usage
- Set request limits in Google Cloud Console
- Never commit `.env.local` to version control

## Contributing 🤝

Contributions are welcome! Please feel free to submit a Pull Request.

## License 📄

This project is open source and available under the MIT License.

## Support 💬

For issues and questions, please open an issue on GitHub.

---

**Built with ❤️ using AI & Modern Web Technologies**
