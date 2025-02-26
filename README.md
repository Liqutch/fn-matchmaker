## OVERVIEW
This Python script interacts with Fortnite's matchmaking services using Epic Games' official APIs. It automates the matchmaking process by generating necessary authentication tokens, requests and establishing a WebSocket connection to Epic Games' matchmaking servers.

## USAGE
To use this project, ensure you have Python installed along with the required dependencies. Follow the steps below to set up and integrate it into your own project.

1. **Make sure you have Python 3.8+ installed. Then, install the required libraries using:**
   
   ```
   pip install aiohttp websockets
   ```
2. **Include the Script in Your Project**

    You can directly import and use the DontMessWithMMS class in your Python project like in the example:
    ```py
    from matchmaker import DontMessWithMMS
    import asyncio

    async def main():
        mms = DontMessWithMMS(
            account_ids=["MATCHMAKING_ACCOUNT_IDS"],
            exchange_code="CLIENT_EXCHANGE_CODE",
            playlist="CLIENT_PLAYLIST",
            party_id="CLIENT_PARTY_ID",
            region="PARTY_REGION",
            fill=False #Recommended
        )
        await mms.start()
    
    asyncio.run(main())
    ```

## DISCLAIMER
This project interacts with Fortnite's matchmaking and game session services through Epic Games' official APIs. However, please note that improper or excessive use of these APIs may violate Epic Games' Terms of Service. While efforts have been made to align this project with best practices and Epic Games' policies, using third-party tools always carries some level of risk.

I take no responsibility for any consequences resulting from the use of this project, including but not limited to:

- Temporary or permanent bans from Fortnite.
- Loss of in-game items or progress.
- Restrictions on your Epic Games account.

It is your responsibility to use this project within the limits of Epic Games' policies. Proceed at your own risk, and be fully aware of the potential consequences. By using this project, you acknowledge and accept any risks involved.

## CONTACT
If you want to, you can contact me from the links below.

[![Discord](https://img.shields.io/badge/Discord-%237289DA.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.com/users/341886629142593537)
[![Website](https://img.shields.io/badge/🔗%20LIQUTCH.DEV-white.svg?style=for-the-badge&logo=link&logoColor=black&color=EDF2F7)](https://liqutch.dev)
[![X](https://img.shields.io/badge/X-%23000000.svg?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/Liqutch)
