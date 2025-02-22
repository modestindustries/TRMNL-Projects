# TRMNL-KEXP-Playlist

This is a [TRMNL](https://usetrmnl.com/) plug-in that displays [KEXP's](https://kexp.org) Real Time Playlist.

This is not endorsed by the fine folks at KEXP in any way. 

![full_screen](https://github.com/user-attachments/assets/9959d8a8-4451-4361-bac1-bef1f6110bc5)

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
**Form Fields**:
```
- keyname: airtime_timezone
  field_type: select
  options:
  - 'My local time zone'
  - 'KEXP Seattle time zone'
  name: Time Zone
  description: Time zone to use for song air times
  help_text: Your TRMNL's time zone, or KEXP Seattle's.
  default: my_local_time_zone
  ```
**Remove bleed margin?**: No

2. Copy / paste the markup to each of the appropriate layouts.