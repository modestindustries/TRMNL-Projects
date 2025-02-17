# TRMNL-KEXP-Playlist

This is a [TRMNL](https://usetrmnl.com/) plug-in that polls [KEXP](https://kexp.org)
's public API, and displays their Real Time Playlist.

This is not endorsed by the fine folks at KEXP in any way. 

![full_screen](https://github.com/user-attachments/assets/9959d8a8-4451-4361-bac1-bef1f6110bc5)

*Strategy*: Polling
*Polling URL*: https://api.kexp.org/v2/plays/
*Polling Verb*: GET
*Polling Headers*: 
```{
  "authorization":"bearer xxx",
  "content-type":"application/json"
}```