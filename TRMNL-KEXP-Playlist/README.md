# TRMNL-KEXP-Playlist

This is a [TRMNL](https://usetrmnl.com/) plug-in that displays [KEXP's Real Time Playlist](https://kexp.org/playlist/).

This is not endorsed by the fine folks at [KEXP](https://kexp.org) in any way. 

![alt text](https://github.com/modestindustries/TRMNL-Projects/blob/main/TRMNL-KEXP-Playlist/images/full_screen.jpg)

## Setup

1. Set up as a Private Plugin, with the following settings:

**Strategy**: Polling\
**Polling URL**: https://api.kexp.org/v2/plays/ \
**Polling Verb**: GET\
**Polling Headers**:
```
{
  "authorization":"bearer",
  "content-type":"application/json"
}
```
**Remove bleed margin?**: No

2. Copy / paste the markup to each of the appropriate layouts.

## Notes
- Airtimes, shown above each track, will be local to you, depending on the Time Zone you've set in usetrml.com.