<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SA EARNING ZONE</title>

<script src='//libtl.com/sdk.js' data-zone='10852660' data-sdk='show_10852660'></script>

<style>
body{
    margin:0;
    font-family:Arial;
    background:#000;
    color:#fff;
}

/* CENTER BOX */
.container{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
}

/* TITLE */
h1{
    color:#00ff88;
    font-size:20px;
    margin-bottom:20px;
}

/* WATCH BUTTON */
.watch-btn{
    width:220px;
    padding:15px;
    border:none;
    border-radius:12px;
    background:#1a1a1a;
    color:#fff;
    font-weight:bold;
    cursor:pointer;
    border:1px solid #2a2a2a;
    transition:0.2s;
}

.watch-btn:hover{
    background:#00ff88;
    color:#000;
}

/* COUNTER */
.counter{
    margin-top:15px;
    font-size:14px;
    color:#aaa;
}

/* DEVELOPER BUTTON (BOTTOM RIGHT) */
.dev-btn{
    position:fixed;
    right:15px;
    bottom:15px;
    padding:8px 12px;
    font-size:12px;
    border:none;
    border-radius:8px;
    background:#111;
    color:#fff;
    border:1px solid #2a2a2a;
    cursor:pointer;
}

.dev-btn:hover{
    background:#00ff88;
    color:#000;
}
</style>
</head>

<body>

<div class="container">

    <h1>𝐒𝐀 𝐄𝐀𝐑𝐍𝐈𝐍𝐆 𝐙𝐎𝐍𝐄</h1>

    <!-- WATCH AD BUTTON -->
    <button class="watch-btn" onclick="watchAd()">𝐖𝐀𝐓𝐂𝐇 𝐀𝐃</button>

    <!-- COUNTER -->
    <div class="counter">
        Ads Watched: <span id="count">0</span>
    </div>

</div>

<!-- DEVELOPER BUTTON -->
<button class="dev-btn" onclick="window.open('https://t.me/@Sayem191 ','_blank')">
    𝐃𝐄𝐕𝐋𝐎𝐏𝐄𝐑
</button>

<script>
let count = localStorage.getItem("adCount") || 0;
document.getElementById("count").innerText = count;

function watchAd(){
    if(typeof show_10852660 === "function"){
        show_10852660();

        // increase counter
        count++;
        localStorage.setItem("adCount", count);
        document.getElementById("count").innerText = count;
    } else {
        alert("Ad load হয়নি!");
    }
}
</script>

</body>
</html>
