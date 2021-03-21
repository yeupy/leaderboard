# Getting Started
Implemented with springboot, gradle, mybatis, h2database.
JUnit5 is used for unit tests.

### Functions Implemented
1. API to return total number of player 
    - GET /stat
2. API to return tier of a player
    - GET /player/{id}
3. API to return list of top 10 players
    - GET /player/top
4. API to return list of players near given player's id.  eg) If playerId is 5 and range of 5 is given.  You are required to find 5 higher rank players and 5 lower rank players
    - GET /player/nearby/{id}
5. API to update/add a player (Leaderboard should also be updated)
    - PUT /player/{id} (Update)
    - POST /player/{id} (Add)
6. API to delete a player
    - DEL /player/{id}

**Remarks**
   - Rank and Tier are non-persistent, instead, they are computed on request.
   - Initial data is not loaded when testing.
    
### Guides
**Build (including test)**

..\leaderboardtest> gradlew build

**Build (excluding test)**

..\leaderboardtest> gradlew build -x test

**Test**

..\leaderboardtest> gradlew test

**Run**

..\leaderboardtest> gradlew bootRun

Server URL -> http://localhost:8080/


### Comments
Too bad, almost ran outta time to discuss anything about designs and thoughts :( I wish I had more time to perfect this task, but yet enjoyed it very much. Thank you for your time. Have a nice day~