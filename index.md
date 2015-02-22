---
title       : Testing Sabermetrics and Conventional Baseball Statistics
subtitle    : Tool to see how well sabermetrics and conventional baseball statistics predict team statistics
author      : Owen Byrne
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : standalone    # {standalone, draft}
knit        : slidify::knit2slides

---

## History of Sabermetrics

1. Bill James disliked conventional baseball statistics because they weren't actually useful
2. Invented his own stats - called "sabermetrics".
3. Concept made famous by "Moneyball."
4. "Runs Created" was the first "sabermetric"

---

## Runs Created

1. Compares individual players to estimate their value to their team.
2. Simple Example - Miguel Tejada was the American League Most Valuable Player in 2002 (determined by voting)
3. Use Advanced Runs Created (using all readily available statistics) to rank AL hitters

---

## American League Hitters (2002) ranked by Advanced Runs Created


```
##       playerID teamID RunsCreatedAdvanced
## 1136 thomeji01    CLE            154.9049
## 901  rodrial01    TEX            153.3114
## 1252 giambja01    NYA            150.2978
## 897  palmera01    TEX            128.1129
## 1287 ramirma02    BOS            127.3876
## 1167 ordonma01    CHA            127.1339
## 1251 soriaal01    NYA            126.2672
## 1255 willibe02    NYA            124.9896
## 1192 delgaca01    TOR            120.7075
## 1059 beltrca01    KCA            115.2039
## 1284 garcino01    BOS            115.0974
## 965  tejadmi01    OAK            113.7712
## 927  olerujo01    SEA            113.1961
## 1063 sweenmi01    KCA            111.5551
## 994  anderga01    ANA            110.6558
```

---

## Conclusion

1. According to "AdvancedRunsCreated", Miguel Tejada (tejadmi01 OAK) was only the 12th best hitter in the American League in 2002. Jim Thome (thomeji01    CLE), Alex Rodriguez (rodrial01    TEX) or Jason Giambi (giambja01    NYA) would have been better choices for American League MVP.

### Shiny Application
1. By aggregating the players on the team, essentially bypass the main purpose of Sabermetrics
2. Nearly all statistics when aggregated provide predictive value of team results
3. One exception is "triples" - most likely because they're pretty rare.
4. But still a useful validation of Sabermetrics
5. [Further Reading](http://en.wikipedia.org/wiki/Sabermetrics)
