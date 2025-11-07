# Chime Update Notes

This repository hosts the dynamic update notes for [Chime](https://chime-app.com) - the ADHD-friendly meeting reminder app for macOS.

## What is this?

Chime fetches update notes from this repository to show users what's new without requiring an app update. This allows us to:
- Provide detailed release notes
- Share tips and tricks
- Announce upcoming features
- Communicate with users between releases

## File Structure

- `update-notes.json` - The main update notes file that Chime fetches
- `archive/` - Historical update notes for reference

## How to Update

1. Edit `update-notes.json` with the new content
2. Commit and push to the main branch
3. Changes appear in the app immediately (no app update needed!)

## JSON Format

```json
{
  "version": "1.0.0",
  "releaseDate": "January 2025",
  "items": [
    {
      "icon": "sparkles",
      "title": "Feature Name",
      "description": "What's new or improved",
      "category": "feature"
    }
  ]
}
```

## Available Icons

All [SF Symbols](https://developer.apple.com/sf-symbols/) are supported. Common ones:
- `sparkles` - New features
- `checkmark.circle.fill` - Bug fixes
- `arrow.up.circle.fill` - Improvements
- `paintbrush.fill` - UI updates
- `bell.badge.fill` - Notifications
- `lock.shield.fill` - Security

## Version Targeting

Use `minAppVersion` and `maxAppVersion` to target specific app versions:

```json
{
  "minAppVersion": "1.0.0",
  "maxAppVersion": "1.0.5"
}
```

## Update Schedule

- **Launch Day**: Detailed feature list
- **Week 1**: Power user tips
- **Week 2-3**: Hidden features
- **Monthly**: Seasonal tips & community highlights

## Testing

To test changes before users see them:
1. Create a branch
2. Update the JSON
3. Test with debug build pointing to branch
4. Merge when ready

---

© 2025 Chime. For questions, contact support@chime-app.com