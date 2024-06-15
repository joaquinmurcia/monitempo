# monitempo

Activity monitor and classifier based on computer (Mac) screen time reports and an ESPresense + Home Assistant BLE
device location system

## Get activity reports

## Screen time

- In Mac you have Screen Time, but exporting the data is forensics-level
  difficult https://www.mac4n6.com/blog/2018/8/5/knowledge-is-power-using-the-knowledgecdb-database-on-macos-and-ios-to-determine-precise-user-and-application-usage
  and it is in a complicated database format.

### Toggl Track
I've decided to use Toggl Track because the export is in a comfortable .json format, I had already used it for time
  tracking, it is free, and can track apps and websites both on phone and computer. How to
  export: https://support.toggl.com/en/articles/2564936-exporting-data.

You can export both:
- Time entries: the thing you actually start and stop tracking manually. Exported in csv
- Timeline: the app and website activity. This is what we are interested in. Exported in json

Problems:
- Lacks automatic categorization of activities
- Does not seem to track idle time from computer at all

### TODOs

- [ ] Install and track in work computer and phone, too

### Personal notes

- You have a relevant bookmarks folder for this project. It contains things such as why WiFi does not work properly on
  your ESP32's
    - Even having the door of your room open makes a difference towards router connectivity.

### Future features

- [ ] Real-time monitoring and classification
- [ ] Decision-making-related insights (e.g. worth of time spent on a given activity)