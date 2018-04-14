# docker-light-mc-crawler
A Docker wrapper for light-mc-crawler

## How to use
1) Customise config.json
2) run `docker build -t dockerlightmccrawler .`
3) run `docker run -it dockerlightmccrawler`

## Example output

```
> docker-mixed-content-finder@1.1.0 start /app
> light-mc-crawler --url https://www.example.com/music --config config.json


Http link on https://www.example.com/music
  http://www.example.com/music/resources/idt-sh/dancing
  http://www.example.com/music/resources/idt-sh/clubs
  http://www.example.com/music/musictime
  http://www.example.com/music/musictime
  http://www.example.com/music/10628994
  http://www.example.com/music/help-41670342

Mixed Content
https://www.example.com/music ✗ is-on-https - Does not use HTTPS
   http://www.petmd.com/sites/default/files/petmd-cat-happy-10.jpg
   http://www.argospetinsurance.co.uk/assets/uploads/2017/12/cat-pet-animal-domestic-104827.jpeg


Lighthouse Summary
  Total Pages Scanned: 1
  Total Auditing Time: 22905 ms
  Average Page Audit Time: 20611 ms
  Total Audits Passed: 0 ✓
  Total Violations:
    Mixed Content: 2 ✗
