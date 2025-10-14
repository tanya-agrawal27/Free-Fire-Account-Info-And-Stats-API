![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-269539?style=for-the-badge&logo=nginx&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![CI/CD](https://img.shields.io/badge/CI/CD-4CAF50?style=for-the-badge&logo=continuousintegration&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-02569B?style=for-the-badge&logo=rest&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=json&logoColor=white)
![Axios](https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

# Free Fire Account Info API - HL Gaming Official

The **HL Gaming Official Free Fire API (All-in-One)** is a powerful and secure RESTful JSON API that allows developers to access Free Fire player account details across more than 14 regions worldwide. It provides accurate, real-time player data including level, rank, guild, region, and overall profile information through a single, unified endpoint. Designed for reliability, simplicity, and high performance, this API is ideal for game dashboards, automation tools, and data analysis systems.

Developers can integrate the API seamlessly using standard GET requests and retrieve structured JSON responses ready for frontend or backend usage. Authentication is mandatory for all requests using an assigned **API key** and **developer UID**, ensuring security and controlled access. The system is optimized for global use with multi-region endpoint routing for faster response times and enhanced data consistency.

All users must include proper parameters such as `PlayerUid`, `region`, `useruid`, and `api` in their requests to obtain a valid response. For official documentation, key generation, and region details, please visit the HL Gaming Official website and the API documentation page.
## GET Request - Free Fire Account Information

The **HL Gaming Official Free Fire API (All-in-One)** allows developers to retrieve complete account details of any Free Fire player using a simple **GET request**. This endpoint provides structured JSON responses containing all essential information such as player stats, rank data, guild info, credit score, pet details, and more.

### Base Endpoint
```
https://proapis.hlgamingofficial.com/main/games/freefire/account/api
```

### Method
```
GET
```

### Required Query Parameters
| Parameter | Description |
|------------|--------------|
| `sectionName` | The data section to retrieve. Use `AllData` to fetch full account details. |
| `PlayerUid` | The unique identifier of the Free Fire player. |
| `region` | The player’s region code (e.g., pk, ind, br, sg, us, ru). |
| `useruid` | Your developer UID from the HL Gaming dashboard. |
| `api` | Your secret API key for authorization. Obtain it from [https://www.hlgamingofficial.com/p/api.html](https://www.hlgamingofficial.com/p/api.html). |

### Example Request
```bash
curl -X GET "https://proapis.hlgamingofficial.com/main/games/freefire/account/api?sectionName=AllData&PlayerUid=9351564274&region=pk&useruid={your_useruid}&api={your_api_key}"
```

### Example Response
```json
{
  "source": "HL Gaming Official",
  "endpoint": "AllData",
  "result": {
    "AccountInfo": {
      "AccountAvatarId": 902046036,
      "AccountBPBadges": 33,
      "AccountBPid": 1001000083,
      "AccountBannerId": 901048012,
      "AccountCreateTime": 1715887148,
      "AccountEXP": 475955,
      "AccountLastLogin": 1744559723,
      "AccountLevel": 54,
      "AccountLikes": 2303,
      "AccountName": "༄ᴾᴿᴼ✿ʜᴀʀᴏᴏɴ࿐",
      "AccountRegion": "pk",
      "AccountSeasonId": 44,
      "AccountType": 1,
      "BrMaxRank": 321,
      "BrRankPoint": 3633,
      "CsMaxRank": 309,
      "CsRankPoint": 32,
      "EquippedWeapon": [907104815],
      "ReleaseVersion": "OB48",
      "ShowBrRank": true,
      "ShowCsRank": true
    },
    "AccountProfileInfo": {
      "EquippedOutfit": [204000345, 203046040, 211048038, 205046027, 211036046, 214000000],
      "EquippedSkills": [16, 6201, 8, 1, 16, 1806, 8, 2, 16, 6906, 8, 3, 16, 5206]
    },
    "GuildInfo": {
      "GuildCapacity": 40,
      "Guildid": "3072889293",
      "GuildLevel": 4,
      "GuildMember": 39,
      "GuildName": "Mᴋ᭄Gᴀᴍɪɴɢ❤︎",
      "GuildOwner": "7144371811"
    },
    "captainBasicInfo": {
      "accountId": "7144371811",
      "accountType": 1,
      "badgeCnt": 51,
      "badgeId": "1001000083",
      "createAt": "1670344853",
      "csMaxRank": 321,
      "csRank": 321,
      "csRankingPoints": 101,
      "exp": 831967,
      "headPic": "902000120",
      "lastLoginAt": "1744363838",
      "level": 59,
      "liked": 2757,
      "maxRank": 324,
      "nickname": "Mᴋ᭄LEADER❤︎",
      "pinId": "910040001",
      "rank": 324,
      "rankingPoints": 5323,
      "region": "pk",
      "releaseVersion": "OB48",
      "seasonId": 44,
      "showBrRank": true,
      "showCsRank": true,
      "title": 904190040
    },
    "creditScoreInfo": {
      "creditScore": 100,
      "periodicSummaryEndTime": "1744860016",
      "periodicSummaryStartTime": "1744600816"
    },
    "petInfo": {
      "exp": 504,
      "id": 1300000101,
      "isSelected": true,
      "level": 4,
      "selectedSkillId": 1315000009,
      "skinId": 1310000102
    },
    "socialinfo": {
      "AccountLanguage": "Language_English",
      "AccountPreferMode": "Prefermode_br",
      "AccountSignature": "••°FOUNDER & CEO OF HL GAMING OFFICIAL WEBSITE°••"
    }
  },
  "usage": {
    "usedToday": 5,
    "dailyLimit": 50,
    "remainingToday": 45
  }
}
```

### Notes
- Always include valid credentials (`useruid` and `api`) to avoid authentication errors.
- The `sectionName=AllData` parameter fetches full account information in a single call.
- Data refreshes automatically based on Garena’s live servers.
- To generate your **API key** and **developer UID**, visit:  
  [https://www.hlgamingofficial.com/p/api.html](https://www.hlgamingofficial.com/p/api.html)

  
## Full Documentation and Advanced Usage

The **HL Gaming Official Free Fire API (All-in-One)** offers a complete and advanced documentation hub for developers who need deeper integration options, advanced filtering, and access to multiple Free Fire data endpoints beyond the `AllData` section.

The documentation includes:
- Detailed descriptions of each API endpoint and response object  
- Inline code examples in multiple languages (Node.js, Python, PHP, etc.)  
- Error handling and troubleshooting guides  
- Parameter breakdowns for `AccountInfo`, `GuildInfo`, `RankData`, `CreditScore`, and other sections  
- Usage limits, rate control details, and best practices for optimized API calls  

Developers are strongly encouraged to refer to the full documentation for professional implementation, production-level integration, and secure API handling.

For the complete API reference and technical guide, visit the official documentation page:  
[https://www.hlgamingofficial.com/p/free-fire-api-data-documentation.html](https://www.hlgamingofficial.com/p/free-fire-api-data-documentation.html)

## Player Statistics Data (Solo, Duo, Squad)

The **HL Gaming Official Free Fire Player Stats API** provides in-depth gameplay analytics for each player, including detailed combat performance across **Solo**, **Duo**, and **Squad (Quad)** modes. This data allows developers to build leaderboards, player comparison tools, and advanced analytical dashboards.

Each request returns structured data in JSON format, summarizing gameplay performance such as total kills, deaths, headshots, wins, distance traveled, survival time, and more — all sourced directly from Free Fire’s live servers.

### Example Data Response

```json
"playerStats": {
  "duostats": {
    "accountid": "12345678",
    "detailedstats": {
      "damage": 69400,
      "deaths": 81,
      "distancetravelled": 321696,
      "headshotkills": 18,
      "headshots": 44,
      "highestkills": 31,
      "knockdown": 167,
      "pickups": 4728,
      "revives": 12,
      "roadkills": 8,
      "survivaltime": 55504,
      "topntimes": 45
    },
    "gamesplayed": 95,
    "kills": 222,
    "wins": 14
  },
  "quadstats": {
    "accountid": "12345678",
    "detailedstats": {
      "damage": 4978192,
      "deaths": 2150,
      "distancetravelled": 15777516,
      "headshotkills": 854,
      "headshots": 2207,
      "highestkills": 23,
      "knockdown": 8733,
      "pickups": 265771,
      "revives": 1778,
      "roadkills": 19,
      "survivaltime": 2711693,
      "topntimes": 2352
    },
    "gamesplayed": 3771,
    "kills": 9881,
    "wins": 1621
  },
  "solostats": {
    "accountid": "12345678",
    "detailedstats": {
      "damage": 355099,
      "deaths": 283,
      "distancetravelled": 1405443,
      "headshotkills": 162,
      "headshots": 243,
      "highestkills": 34,
      "pickups": 24604,
      "roadkills": 24,
      "survivaltime": 231765,
      "topntimes": 222
    },
    "gamesplayed": 381,
    "kills": 1279,
    "wins": 98
  }
}
```

### Data Explanation

| Field | Description |
|--------|--------------|
| `gamesplayed` | Total matches played in that mode. |
| `wins` | Total matches won. |
| `kills` | Total player eliminations. |
| `damage` | Total cumulative damage dealt. |
| `deaths` | Total number of times the player was eliminated. |
| `headshotkills` | Number of kills by headshot. |
| `survivaltime` | Total survival time across matches (in seconds). |
| `topntimes` | Number of times the player finished in the top N placements. |

### Usage

To fetch this data, use our dedicated **Player Stats API**, which provides comprehensive and up-to-date performance data for every registered Free Fire player.

👉 Access the detailed Player Stats API documentation here:  
[https://www.hlgamingofficial.com/p/free-fire-player-stats-api.html](https://www.hlgamingofficial.com/p/free-fire-player-stats-api.html)

## Free Fire Likes Generator API

The **HL Gaming Official Free Fire Likes Generator API** allows developers to **send or simulate player likes** to a Free Fire account securely through an authenticated request. This endpoint enables automated like generation for engagement systems, community events, or reward-based integrations while ensuring proper validation and daily claim limits.

Each player can only receive likes **once every 24 hours**, and all actions are tracked for transparency through your HL Gaming Developer Dashboard.

---

### Example Responses

#### Already Claimed

```json
{
  "source":"HL Gaming Official",
  "endpoint":"data/likes",
  "result":{
    "LikesAfterCommand":6233,
    "LikesBeforeCommand":6233,
    "LikesGivenByAPI":0,
    "PlayerNickname":"PlayerOne",
    "TokensUsed":41,
    "UID":8651617771,
    "status":2
  },
  "message":"Hello PlayerOne, it looks like you've already claimed your daily likes within the last 24 hours. Please try again after 24 hours. Thank you for understanding!",
  "usage":{"usedToday":53,"dailyLimit":100,"remainingToday":47}
}
```

#### Successful Grant

```json
{
  "source":"HL Gaming Official",
  "endpoint":"data/likes",
  "result":{
    "LikesAfterCommand":6233,
    "LikesBeforeCommand":6193,
    "LikesGivenByAPI":40,
    "PlayerNickname":"PlayerOne",
    "TokensUsed":41,
    "UID":8651617771,
    "status":1
  },
  "message":"Hello PlayerOne, you’ve successfully received 40 new likes! You had 6193 before, and now you have 6233. Thank you for choosing HL Gaming Official!",
  "usage":{"usedToday":52,"dailyLimit":100,"remainingToday":48}
}
```

---

### Response Fields Explained

| Field | Description |
|--------|--------------|
| `LikesBeforeCommand` | The total number of likes before the API request. |
| `LikesAfterCommand` | The total number of likes after the API request. |
| `LikesGivenByAPI` | Number of likes successfully granted by the API. |
| `PlayerNickname` | The player's nickname as retrieved from the server. |
| `status` | Indicates whether the request was successful (1) or already claimed (2). |
| `usage` | Provides daily API usage statistics for your account. |

---

### Usage Policy
- Each account can **claim likes once per 24 hours**.
- Unauthorized API usage or spamming requests may lead to **temporary suspension**.
- Use responsibly in accordance with **HL Gaming Official Terms of Service**.

👉 Access the full documentation here:  
[https://www.hlgamingofficial.com/p/free-fire-likes-generator-api.html](https://www.hlgamingofficial.com/p/free-fire-likes-generator-api.html)

## Free Fire Account UID Validation API

The **HL Gaming Official Free Fire UID Validation API** provides a powerful, real-time verification system that ensures a given Free Fire UID belongs to a valid player across Garena’s global network. It’s perfect for use in **leaderboards**, **tournament registration**, **reward systems**, and any workflow that depends on confirming player authenticity.

This API is backed by an **optimized caching layer** and **low-latency proxy system**, ensuring that each validation request executes in milliseconds — even under high load — without overloading upstream Garena endpoints.

---

### Base Endpoint

```
https://proapis.hlgamingofficial.com/main/games/freefire/validation/api
```

---

### GET Example

```bash
# GET request with query parameters
curl "https://proapis.hlgamingofficial.com/main/games/freefire/validation/api\
?sectionName=freefireValidation\
&useruid=dev123UID\
&api=abcDEFkey123\
&uid=12345678\
region=SG"
```

**Parameter Explanation:**

| Parameter | Description |
|------------|-------------|
| `sectionName` | Must always be set to **freefireValidation** for this endpoint. |
| `useruid` | Your unique developer identifier from the HL Gaming Official Dashboard. |
| `api` | Your private API key for authentication. Keep it secure. |
| `uid` | The Free Fire player UID you want to validate. |
| `region` | Player’s region code (e.g., `SG` for Singapore, `BR` for Brazil, `PK` for Pakistan). |

> **Tip:** Use `GET` for quick manual testing or debugging, but for production environments, prefer **POST requests** to keep your API key hidden and more secure.

---

### Example Responses

#### Valid UID

```json
{
  "source": "FreeFire Validation",
  "result": {
    "uid": "12345678",
    "region": "SG",
    "valid": true,
    "message": "UID is valid.",
    "details": "User 'FB:ㅤ@GMRemyX' exists in region 'SG' and is at level 67.",
    "AccountName": "FB:ㅤ@GMRemyX",
    "AccountRegion": "SG",
    "AccountLevel": 67
  },
  "usage": {
    "usedToday": 2,
    "dailyLimit": 999,
    "remainingToday": 997
  }
}
```

#### Invalid UID

```json
{
  "source": "FreeFire Validation",
  "result": {
    "uid": "123745678",
    "region": "SG",
    "valid": false,
    "message": "The UID you entered is not valid."
  },
  "usage": {
    "usedToday": 5,
    "dailyLimit": 999,
    "remainingToday": 994
  }
}
```

---

### Response Details

| Field | Description |
|--------|--------------|
| `valid` | Indicates if the UID exists (`true` or `false`). |
| `AccountName` | Player’s in-game name retrieved from Free Fire servers. |
| `AccountLevel` | Player’s current account level. |
| `region` | Region code where the player account exists. |
| `usage` | Real-time quota tracking for your daily API usage. |

---

### Developer Notes

- Every request is validated and cached for efficiency.  
- Supports **14+ Garena regions** globally.  
- Ideal for apps and systems needing **instant UID verification**.  
- Invalid or malformed UIDs will return a `valid: false` response.  
- You can monitor daily usage with the `usage` object in the response.

---

👉 For the **full developer documentation** and advanced integration examples, visit:  
[https://www.hlgamingofficial.com/p/free-fire-account-uid-validation-api.html](https://www.hlgamingofficial.com/p/free-fire-account-uid-validation-api.html)


## Support & Contact

If you experience any technical issues, encounter authentication errors, or require help with API integration, the **HL Gaming Official Support Team** is available to assist you. We handle bug reports, feature requests, and developer onboarding for the Free Fire API (All-in-One).

You can contact us through any of the following methods:

- 📩 **Email Support:** [support@hlgamingofficial.com](mailto:support@hlgamingofficial.com)  
- 🌐 **Official Contact Page:** [HL Gaming Official Contact](https://www.hlgamingofficial.com/p/contact-us.html)  
- 💬 **Community Help & Feedback:** Available through our Discord and Telegram channels (listed on the contact page).  

Our support team typically responds within **24–48 hours**. For business or partnership inquiries, please include your project details and estimated request volume to receive prioritized assistance.

---

## License

This API and its related assets are **developed and maintained by HL Gaming Official**.  
All rights are reserved under the **HL Gaming Official License Agreement**.  
Unauthorized use, modification, resale, or redistribution of the API or its source code is strictly prohibited.

Developers may only use this API for **personal, non-commercial, or approved commercial projects** after obtaining written authorization from HL Gaming Official.

For licensing questions or commercial use approval, please contact us at  
📧 [support@hlgamingofficial.com](mailto:support@hlgamingofficial.com)

---

### **Developed & Maintained by HL Gaming Official**
Pioneering reliable, global Free Fire API services for developers and gamers worldwide.
