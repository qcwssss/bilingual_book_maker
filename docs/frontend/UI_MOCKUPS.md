# Bilingual Book Translation Service - MVP UI Mockups

## Overview

This document contains simplified UI mockups for the MVP version of the bilingual book translation service. The MVP focuses on a simple upload → translate → download flow with no user storage or translation history.

## MVP Business Model

- **Anonymous Users**: Free access to Google Translate only
- **Registered Users**: Access to all translation models using their own API keys
- **No Premium Payments**: Users bring their own API keys, no subscription model
- **No Storage**: All files cleaned up after a few hours
- **No History**: No translation tracking or management in MVP

## Color Scheme Reference

- **Primary Blue**: #2563EB (for main actions and navigation)
- **Success Green**: #10B981 (for completed states and downloads)
- **Warning Amber**: #F59E0B (for alerts and attention items)
- **Error Red**: #EF4444 (for errors and cancel actions)
- **Neutral Gray**: #6B7280 (for secondary text and borders)

---

## 1. Landing Page (MVP - Anonymous Users)

**Purpose**: Simple upload interface with Google Translate, registration prompt for more models.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                     │
│  [🌐 TranslateBooks]                                              [Sign Up/Login]  │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│                          📚 Translate Your Books Instantly                         │
│                                                                                     │
│                Transform EPUB, TXT, SRT, and MD files into any language            │
│                                                                                     │
│                     ┌─────────────────────────────────────┐                       │
│                     │                                     │                       │
│                     │    📁 Drop files here or            │                       │
│                     │                                     │                       │
│                     │        [Choose Files]               │                       │
│                     │                                     │                       │
│                     │   Supported: EPUB, TXT, SRT, MD    │                       │
│                     │     files up to 500KB              │                       │
│                     │                                     │                       │
│                     └─────────────────────────────────────┘                       │
│                                                                                     │
│     ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────────────────┐  │
│     │ From Language    │  │ To Language      │  │ Translation Model            │  │
│     │ ┌──────────────┐ │  │ ┌──────────────┐ │  │ ┌──────────────────────────┐ │  │
│     │ │English    ▼│ │  │ │Spanish    ▼│ │  │ │🆓 Google Translate       │ │  │
│     │ └──────────────┘ │  │ └──────────────┘ │  │ └──────────────────────────┘ │  │
│     └──────────────────┘  └──────────────────┘  └──────────────────────────────┘  │
│                                                                                     │
│                        [🔄 Start Translation]                                      │
│                               (Blue Button)                                        │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐  ┌───────────────┐ │
│  │  🆓 Free         │  │ 📁 File Support │  │ 🔒 Secure       │  │ ⚡ Fast       │ │
│  │                 │  │                 │  │                 │  │               │ │
│  │ Google Translate│  │ EPUB, TXT, SRT, │  │ Files cleaned   │  │ Process in    │ │
│  │ No signup needed│  │ MD formats      │  │ after hours     │  │ minutes       │ │
│  │                 │  │ Up to 500KB     │  │                 │  │               │ │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘  └───────────────┘ │
│                                                                                     │
│  ┌─────────────────────────────────────────────────────────────────────────────────┐ │
│  │                     🔑 Want Better Translations?                               │ │
│  │                                                                                 │ │
│  │   Sign up to access ChatGPT-4, Claude, Gemini Flash with your own API keys:   │ │
│  │                                                                                 │ │
│  │   • Higher quality translations                                                │ │
│  │   • Context-aware processing                                                   │ │
│  │   • Use your existing API subscriptions                                        │ │
│  │   • No additional costs - you control your usage                              │ │
│  │                                                                                 │ │
│  │                          [Sign Up Free →]                                      │ │
│  │                           (Blue Button)                                        │ │
│  └─────────────────────────────────────────────────────────────────────────────────┘ │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

**Key Elements:**
- Large file upload zone as primary focal point
- Only Google Translate available for anonymous users
- Simple signup prompt for access to more models
- Trust indicators (security, speed, file support)
- No premium payments mentioned

---

## 2. Registered User Interface (MVP)

**Purpose**: Access to all translation models with user's own API keys. Same simple upload flow, no history storage.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                     │
│  [🌐 TranslateBooks]  [API Keys]                            [👤 John] [Logout] ▼  │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│  Welcome back, John! 👋                                                           │
│                                                                                     │
│                          📚 Translate Your Books Instantly                         │
│                                                                                     │
│                     ┌─────────────────────────────────────┐                       │
│                     │                                     │                       │
│                     │    📁 Drop files here or            │                       │
│                     │                                     │                       │
│                     │        [Choose Files]               │                       │
│                     │                                     │                       │
│                     │   Supported: EPUB, TXT, SRT, MD    │                       │
│                     │     files up to 500KB              │                       │
│                     │                                     │                       │
│                     └─────────────────────────────────────┘                       │
│                                                                                     │
│     ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────────────────┐  │
│     │ From Language    │  │ To Language      │  │ Translation Model            │  │
│     │ ┌──────────────┐ │  │ ┌──────────────┐ │  │ ┌──────────────────────────┐ │  │
│     │ │English    ▼│ │  │ │Spanish    ▼│ │  │ │🆓 Google Translate       │ │  │
│     │ └──────────────┘ │  │ └──────────────┘ │  │ │🔑 ChatGPT-4              │ │  │
│     └──────────────────┘  └──────────────────┘  │ │🔑 Claude Sonnet          │ │  │
│                                                  │ │🔑 Gemini Flash           │ │  │
│                                                  │ └──────────────────────────┘ │  │
│                                                  └──────────────────────────────┘  │
│                                                                                     │
│                        [🔄 Start Translation]                                      │
│                               (Blue Button)                                        │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐                   │
│  │ API Key Status  │  │ Quick Setup     │  │ Support         │                   │
│  │                 │  │                 │  │                 │                   │
│  │ ✅ Google       │  │ [🔑 Add API Key]│  │ [📚 Tutorials]  │                   │
│  │ ❌ ChatGPT      │  │ [🔧 Test Keys]  │  │ [💬 Help Chat]  │                   │
│  │ ❌ Claude       │  │ [📖 Quick Guide]│  │ [📧 Contact]    │                   │
│  │ ❌ Gemini Flash │  │                 │  │                 │                   │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘                   │
│                                                                                     │
│  💡 Tip: Models with 🔑 require your own API key. Set them up in API Keys section│
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

**Key Elements:**
- Simplified navigation (no dashboard or history)
- All translation models visible with clear indicators (free vs API key required)
- API key status overview
- Quick setup assistance
- Same simple upload flow as anonymous users

---

## 3. Translation Progress Page (MVP)

**Purpose**: Simple progress tracking with basic status and download link when complete.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                     │
│  [🌐 TranslateBooks]                                      [← Back to Main]         │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│                          Translation in Progress                                    │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                                                                               │  │
│  │  📖 "Pride and Prejudice.epub"                                               │  │
│  │  English → Spanish • Using ChatGPT-4 • 342 KB EPUB • 12 chapters            │  │
│  │  Started: Today, 3:15 PM                                                     │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐ │  │
│  │  │ ████████████████████████████████████████████████████████▓▓▓▓▓▓▓▓▓▓▓▓ │ │  │
│  │  │                           Progress: 83%                                │ │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘ │  │
│  │                                                                               │  │
│  │  🔄 Currently Processing: Chapter 12 - "Family Matters"                      │  │
│  │  ⏱️ Estimated Time Remaining: 2 minutes                                      │  │
│  │                                                                               │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                             💡 Note                                           │  │
│  │                                                                               │  │
│  │  Your file is being processed. You can bookmark this page or save the        │  │
│  │  job ID below to check status later. Files are automatically cleaned up      │  │
│  │  after a few hours.                                                           │  │
│  │                                                                               │  │
│  │  Job ID: TR_2024_0923_1547_A8B9C2                                           │  │
│  │                                                                               │  │
│  │  When complete, your download will be available here.                        │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

**Key Elements:**
- Large progress bar with percentage
- File details integrated into the title line (size, type, chapters)
- Current processing status and time estimate
- Job ID for reference (no dashboard to track in)
- Clear messaging about file cleanup policy
- No action buttons during translation - keep it simple

---

## 4. Translation Complete Page (MVP)

**Purpose**: Simple success state with download button. No feedback collection or detailed metrics.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                     │
│  [🌐 TranslateBooks]                                      [← Back to Main]         │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│                           ✅ Translation Complete!                                 │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                                                                               │  │
│  │  🎉 Your translation is ready!                                               │  │
│  │                                                                               │  │
│  │  📖 "Pride and Prejudice.epub" → "Orgullo y Prejuicio.epub"                │  │
│  │  English → Spanish • Using ChatGPT-4 • 342→378 KB EPUB • 12 chapters       │  │
│  │  Completed: Today, 3:47 PM • Processing time: 32 minutes                    │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐ │  │
│  │  │ ████████████████████████████████████████████████████████████████████ │ │  │
│  │  │                           Progress: 100%                               │ │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘ │  │
│  │                                                                               │  │
│  │                    [📥 Download Translated Book]                             │  │
│  │                           (Large Green Button)                               │  │
│  │                                                                               │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                             💡 Important                                      │  │
│  │                                                                               │  │
│  │  Your translated file will be available for download for a few hours only.   │  │
│  │  Please save it to your device now. Files are automatically cleaned up for   │  │
│  │  security and storage reasons.                                                │  │
│  │                                                                               │  │
│  │  Job ID: TR_2024_0923_1547_A8B9C2                                           │  │
│  │                                                                               │  │
│  │  Want to translate another file? [🔄 Start New Translation]                  │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

**Key Elements:**
- Large download button as primary action
- File details integrated into the title line (original→translated size, type, chapters)
- Clear messaging about temporary file storage
- Quick action to start new translation
- No feedback collection, sharing features, or detailed statistics cards

---

## 5. API Key Management Page (MVP)

**Purpose**: Simple API key setup for registered users to access premium models.

```
┌─────────────────────────────────────────────────────────────────────────────────────┐
│                                                                                     │
│  [🌐 TranslateBooks]  [← Back]                              [👤 John] [Logout] ▼  │
│                                                                                     │
├─────────────────────────────────────────────────────────────────────────────────────┤
│                                                                                     │
│                            API Key Setup                                           │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                                                                               │  │
│  │  🔑 Add your API keys to access premium translation models                   │  │
│  │                                                                               │  │
│  │  Your keys are encrypted and only used for your translations. You control    │  │
│  │  your usage and costs directly through your API provider accounts.           │  │
│  │                                                                               │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                         Available Models                                      │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐ │  │
│  │  │ 🤖 OpenAI (ChatGPT)                                      ✅ Connected   │ │  │
│  │  │                                                                         │ │  │
│  │  │ API Key: sk-...Kx9L (Last 4 shown)                      [🔄 Update]   │ │  │
│  │  │ Status: Active                                           [❌ Remove]   │ │  │
│  │  │                                                                         │ │  │
│  │  │ Available: GPT-3.5 Turbo, GPT-4, GPT-4 Turbo                          │ │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘ │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐ │  │
│  │  │ 🧠 Anthropic (Claude)                                    ❌ Not Setup   │ │  │
│  │  │                                                                         │ │  │
│  │  │ ┌─────────────────────────────────────────────────────────────────────┐ │ │  │
│  │  │ │ API Key: [Enter your Claude API key here...]           │ │ │  │
│  │  │ └─────────────────────────────────────────────────────────────────────┘ │ │  │
│  │  │                                          [💾 Save] [📋 Get Key]       │ │  │
│  │  │                                                                         │ │  │
│  │  │ Available: Claude 3 Haiku, Claude 3 Sonnet, Claude 3 Opus             │ │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘ │  │
│  │                                                                               │  │
│  │  ┌─────────────────────────────────────────────────────────────────────────┐ │  │
│  │  │ 🎯 Google AI (Gemini Flash)                              ❌ Not Setup   │ │  │
│  │  │                                                                         │ │  │
│  │  │ ┌─────────────────────────────────────────────────────────────────────┐ │ │  │
│  │  │ │ API Key: [Enter your Google AI API key here...]        │ │ │  │
│  │  │ └─────────────────────────────────────────────────────────────────────┘ │ │  │
│  │  │                                          [💾 Save] [📋 Get Key]       │ │  │
│  │  │                                                                         │ │  │
│  │  │ Available: Gemini Flash (1.5), Gemini Flash (2.0)                     │ │  │
│  │  └─────────────────────────────────────────────────────────────────────────┘ │  │
│  │                                                                               │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
│  ┌───────────────────────────────────────────────────────────────────────────────┐  │
│  │                           Quick Start Guide                                   │  │
│  │                                                                               │  │
│  │  🔗 Get API Keys: [🤖 OpenAI →]  [🧠 Anthropic →]  [🎯 Google AI →]         │  │
│  │                                                                               │  │
│  │  📋 Steps:                                                                   │  │
│  │  1. Click a provider link above                                              │  │
│  │  2. Create account or sign in                                                │  │
│  │  3. Generate new API key                                                     │  │
│  │  4. Copy and paste it above                                                  │  │
│  │  5. Start translating with better models!                                    │  │
│  │                                                                               │  │
│  └───────────────────────────────────────────────────────────────────────────────┘  │
│                                                                                     │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐                   │
│  │ Security        │  │ Your Control    │  │ Support         │                   │
│  │                 │  │                 │  │                 │                   │
│  │ 🔐 Encrypted    │  │ 💰 You pay APIs │  │ 💬 Help Chat    │                   │
│  │ 🚫 Not stored   │  │ ⚙️ Your usage   │  │ 📚 Tutorials    │                   │
│  │ 🛡️ Secure       │  │ 📊 Direct bills │  │ 📧 Contact      │                   │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘                   │
│                                                                                     │
└─────────────────────────────────────────────────────────────────────────────────────┘
```

**Key Elements:**
- Service status indicators (connected/not setup)
- Simple API key input forms
- Direct links to API key providers
- Clear messaging about user control over costs
- Simplified navigation without complex dashboards

---

## MVP Design Implementation Notes

### Core Principles
1. **Simplicity First**: Clean, uncluttered interface focusing on core upload → translate → download flow
2. **No Storage Complexity**: Clear messaging that files are temporary and cleaned up automatically
3. **User Control**: Transparent about API keys, costs, and no hidden fees
4. **Progressive Enhancement**: Anonymous users get basic functionality, registered users get premium models

### Visual Hierarchy
1. **Primary Actions**: Large, prominent buttons (file upload, download, start translation)
2. **Secondary Actions**: Medium buttons (cancel, refresh, setup)
3. **Tertiary Actions**: Small buttons and links (help, tutorials)

### Color Usage (Simplified)
- **Blue (#2563EB)**: Main actions, navigation, primary buttons
- **Green (#10B981)**: Success states, completed translations, download buttons
- **Red (#EF4444)**: Errors, cancellation, removal actions
- **Gray (#6B7280)**: Secondary text, borders, disabled states

### Key Differences from Full Version
- **No Dashboard**: Simple main page with upload form
- **No History**: No translation tracking or management
- **No Complex User Management**: Basic signup/login, API key setup
- **No Subscription UI**: No payment flows, premium tiers, or billing
- **Temporary Storage**: Clear messaging about file cleanup
- **BYOK Model**: Users bring own API keys, no service-provided credits

### Responsive Behavior
- **Mobile**: Single column layout, large touch targets
- **Desktop**: Centered layout with clear visual hierarchy

This MVP mockup set provides a foundation for implementing a simple, user-controlled translation service without the complexity of subscription management, file storage, or detailed analytics.