# I – Introducing this year's Steam Event
![image](https://user-images.githubusercontent.com/104601534/175810831-f4fdf3e4-3724-403e-aca3-e63b097e2b3e.png)

<br>

Like every year, this year (2022) steam also released a summer event "Steam Summer Sale" with the most delicious reward being animated avatar border and pretty animated background as shown below. However, the process of completing the task is quite difficult and time consuming. So today I will show you how to get all the rewards in 1 minute!

How to get all the rewards of Steam Summer Sale 2022 in 1 minute
<br>
# II- Instructions on how to do it

### 1- Open Steam
![image](https://user-images.githubusercontent.com/104601534/175810278-e40a0812-c57d-440f-b986-dc919ceaddc3.png)
<br>

Log in to your account and go to the Steam Store homepage. You will now see an introduction to the Steam Summer Sale event as shown below
<br>

![image](https://user-images.githubusercontent.com/104601534/175810242-ab333c31-6c7e-468f-876b-790a69950c24.png)


When you scroll down and see the words "Free Fun This Way", please click on it

![image](https://user-images.githubusercontent.com/104601534/175810304-28fb0cf1-db20-4842-9606-930d8547b2df.png)


Then scroll down and click on the word “Jump to Current clue”


Continue to click on “Click me” and click on “Go Find It”. You will now be directed to this event's quest page. Now press “F12” and then click on the Console tab and enter the code below and press enter

![image](https://user-images.githubusercontent.com/104601534/175810483-6264b312-b283-47d6-a217-e1f25a77c716.jpg)


### 2-Enter the auto code
Copy the code below and go back to the steam page just now and paste it in and press enter

```
/* eslint-env browser */
/* global g_sessionID jQuery */


(async() => {
    let delay = (ms) => new Promise((res) => setTimeout(res, ms));
    await jQuery.post("/saleaction/ajaxopendoor", {
        "sessionid": g_sessionID,
        "authwgtoken": jQuery("#application_config").data("userinfo").authwgtoken,
        "door_index": 0,
        "clan_accountid": 41316928,
    });
    for (let link of [
        "/category/arcade_rhythm/?snr=1_614_615_clorthaxquest_1601",
        "/category/strategy_cities_settlements/?snr=1_614_615_clorthaxquest_1601",
        "/category/sports/?snr=1_614_615_clorthaxquest_1601",
        "/category/simulation/?snr=1_614_615_clorthaxquest_1601",
        "/category/multiplayer_coop/?snr=1_614_615_clorthaxquest_1601",
        "/category/casual/?snr=1_614_615_clorthaxquest_1601",
        "/category/rpg/?snr=1_614_615_clorthaxquest_1601",
        "/category/horror/?snr=1_614_615_clorthaxquest_1601",
        "/vr/?snr=1_614_615_clorthaxquest_1601",
        "/category/strategy/?snr=1_614_615_clorthaxquest_1601",
    ]) {
        try {
            let html = await jQuery.get(link);
            await jQuery.post("/saleaction/ajaxopendoor", {
                "sessionid": g_sessionID,
                "authwgtoken": jQuery("#application_config", html).data("userinfo").authwgtoken,
                "door_index": jQuery("#application_config", html).data("capsuleinsert").payload,
                "clan_accountid": 41316928,
                "datarecord": jQuery("#application_config", html).data("capsuleinsert").datarecord,
            });
            console.log("You got a new badge!");
        } catch (e) {
            console.error("Failed to obtain badge!", e);
        } finally {
            await delay(1500);
        }
    }
})();
```

After entering the code, press enter and wait for the code to run to receive the gift. When you run to number 10, it's done

After the code is done, go back to the Store homepage and click “Free Fun This Way” again. Then click on “Jump To Current Clue” then click “Click Me” then click “Your Profile” as shown below

![image](https://user-images.githubusercontent.com/104601534/175810542-a0e788fc-bd2d-4b80-8606-f32f773ec256.png)


### 3 – Apply the theme and enjoy the results
After clicking on “Your Profile” you will be directed to the profile page as shown below. Now you choose "Steam 3000" and press "Save" and you're done!

![image](https://user-images.githubusercontent.com/104601534/175810558-880f3b84-7ae3-4e42-b7cd-201adaa711ea.png)


