<!-- COMPETITION.HTML -->
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#03152d">

<title>LVT | Lyrics Competition</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Playfair+Display:wght@700;800;900&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    min-height:100vh;
    color:white;
    font-family:Inter,Arial,sans-serif;
    background:
        radial-gradient(circle at 50% 20%,#063a86 0%,#031d48 35%,#02132e 72%,#010b1d 100%);
    overflow-x:hidden;
}

/* BLUE LIGHT EFFECTS */

body:before,
body:after{
    content:"";
    position:fixed;
    pointer-events:none;
    z-index:0;
}

body:before{
    width:900px;
    height:900px;
    left:-430px;
    top:40px;
    background:linear-gradient(
        125deg,
        transparent 42%,
        rgba(32,116,255,.30) 47%,
        transparent 50%
    );
    transform:rotate(13deg);
}

body:after{
    width:900px;
    height:900px;
    right:-450px;
    top:40px;
    background:linear-gradient(
        235deg,
        transparent 42%,
        rgba(32,116,255,.30) 47%,
        transparent 50%
    );
    transform:rotate(-13deg);
}

/* HEADER */

.header{
    position:relative;
    z-index:10;
    height:67px;
    background:#08090c;
    border-bottom:2px solid #e6ad25;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:0 43px;
}

.logo-name{
    display:flex;
    align-items:center;
    gap:12px;
    color:#f2b52a;
    font-size:24px;
    font-weight:800;
}

.trophy{
    font-size:29px;
}

.menu{
    width:50px;
    height:46px;
    border:1px solid #dca51e;
    border-radius:10px;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    gap:6px;
}

.menu i{
    display:block;
    width:28px;
    height:2px;
    background:#eab32a;
}

/* MAIN */

.main{
    position:relative;
    z-index:2;
    width:100%;
    max-width:1100px;
    margin:auto;
    padding:38px 30px 35px;
}

/* MICROPHONE */

.microphone{
    position:absolute;
    right:35px;
    top:40px;
    width:180px;
    height:280px;
    transform:rotate(12deg);
    opacity:.95;
}

.mic-body{
    position:absolute;
    left:50px;
    top:5px;
    width:82px;
    height:160px;
    border:5px solid #c58a19;
    border-radius:45px;
    background:
        radial-gradient(circle,#2272c9 1px,transparent 2px);
    background-size:7px 7px;
    box-shadow:
        inset 0 0 20px #001a46,
        0 0 25px rgba(30,128,255,.6);
}

.mic-line{
    position:absolute;
    left:67px;
    top:155px;
    width:48px;
    height:95px;
    border:5px solid #b67a12;
    border-top:0;
    border-radius:0 0 35px 35px;
}

.mic-neck{
    position:absolute;
    left:86px;
    top:225px;
    width:10px;
    height:45px;
    background:#c48a1d;
}

.mic-base{
    position:absolute;
    left:58px;
    top:263px;
    width:70px;
    height:7px;
    border-radius:10px;
    background:#d59a1b;
}

/* LVT */

.lvt{
    text-align:center;
    font-family:"Playfair Display",serif;
    font-size:clamp(90px,15vw,150px);
    line-height:.85;
    letter-spacing:5px;
    color:#f4bd35;
    text-shadow:
        0 2px 0 #8c5d08,
        0 4px 5px #271900,
        0 0 22px rgba(255,190,40,.55);
}

/* LAUREL */

.laurel{
    position:absolute;
    left:90px;
    top:70px;
    color:#e8a91f;
    font-size:105px;
    line-height:1;
    transform:rotate(-20deg);
}

.laurel.right{
    left:auto;
    right:175px;
    transform:scaleX(-1) rotate(-20deg);
}

/* TITLE */

.competition-title{
    position:relative;
    z-index:2;
    text-align:center;
    margin-top:8px;
    font-family:"Playfair Display",serif;
    color:#f2b82d;
    font-size:clamp(34px,5vw,58px);
    line-height:1;
    text-shadow:0 3px 5px #000;
}

/* DATE */

.date{
    width:max-content;
    margin:17px auto 0;
    padding:7px 40px;
    border:1.5px solid #e9ad25;
    border-radius:11px;
    color:#f3b62c;
    font-size:32px;
    font-weight:800;
    background:rgba(2,16,38,.55);
}

/* STARS */

.stars{
    text-align:center;
    margin:10px 0 15px;
    color:#f1b62b;
    font-size:27px;
    letter-spacing:5px;
}

/* DESCRIPTION */

.description{
    text-align:center;
    font-size:19px;
    line-height:1.55;
    color:#f2f2f2;
}

/* LIVE LABEL */

.live-box{
    position:relative;
    width:min(500px,90%);
    margin:27px auto -1px;
    padding:9px 20px;
    text-align:center;
    color:#f2b62b;
    font-size:23px;
    font-weight:800;
    border:1.5px solid #e5ac25;
    border-radius:17px;
    background:#06224a;
    z-index:5;
}

.live-circle{
    display:inline-block;
    width:20px;
    height:20px;
    margin-right:9px;
    vertical-align:-2px;
    background:#f2b52b;
    border-radius:50%;
}

/* TABLE OUTER */

.table-card{
    width:92%;
    margin:auto;
    padding:0 18px 17px;
    border:2px solid #dda91e;
    border-radius:16px;
    background:rgba(2,22,49,.82);
}

/* TABLE */

.table-wrap{
    overflow:hidden;
    border:1.5px solid #e3ad25;
    border-radius:14px;
}

table{
    width:100%;
    border-collapse:collapse;
    table-layout:fixed;
}

thead th{
    height:48px;
    color:#efb62a;
    font-size:18px;
    border-bottom:1px solid #d9a21c;
}

thead th:nth-child(1){
    width:14%;
}

thead th:nth-child(3){
    width:19%;
}

tbody td{
    height:52px;
    border-right:1px solid rgba(221,174,45,.30);
    border-bottom:1px solid rgba(221,174,45,.28);
    text-align:center;
}

tbody tr:last-child td{
    border-bottom:0;
}

tbody td:last-child{
    border-right:0;
}

.rank{
    color:#f0b62a;
    font-size:23px;
    font-weight:800;
}

.name-box{
    width:90%;
    height:35px;
    margin:auto;
    border:1px solid rgba(172,181,194,.55);
    border-radius:8px;
    background:rgba(2,14,31,.70);
}

.name-box input{
    width:100%;
    height:100%;
    border:0;
    outline:0;
    background:transparent;
    color:white;
    text-align:center;
    font-size:14px;
}

.points-box{
    width:70px;
    height:35px;
    margin:auto;
}

.points-box input{
    width:100%;
    height:100%;
    border:0;
    outline:0;
    background:transparent;
    color:#f3b82d;
    text-align:center;
    font-size:20px;
    font-weight:700;
}

/* INFO */

.info{
    width:92%;
    margin:16px auto 0;
    padding:19px 22px;
    border:2px solid #dfa820;
    border-radius:14px;
    background:rgba(3,24,50,.88);
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.info-item{
    display:flex;
    align-items:center;
    justify-content:center;
    gap:12px;
    min-height:65px;
    border-right:1px solid rgba(225,173,35,.55);
}

.info-item:last-child{
    border-right:0;
}

.info-icon{
    font-size:31px;
}

.info-label{
    color:#f0b62b;
    font-size:13px;
    font-weight:700;
    margin-bottom:5px;
}

.info-value{
    color:#fff;
    font-size:16px;
}

/* QUOTE */

.quote{
    text-align:center;
    margin:22px auto 0;
    width:90%;
    color:#e9ae28;
    font-size:16px;
    font-style:italic;
}

/* MOBILE */

@media(max-width:700px){

    .header{
        height:66px;
        padding:0 14px;
    }

    .logo-name{
        font-size:17px;
    }

    .trophy{
        font-size:23px;
    }

    .menu{
        width:46px;
        height:42px;
    }

    .main{
        padding:28px 8px 30px;
    }

    .microphone{
        display:none;
    }

    .laurel{
        display:none;
    }

    .lvt{
        font-size:90px;
    }

    .competition-title{
        font-size:32px;
    }

    .date{
        font-size:25px;
        padding:7px 25px;
    }

    .description{
        font-size:16px;
    }

    .live-box{
        width:88%;
        font-size:18px;
        padding:9px 12px;
    }

    .table-card{
        width:94%;
        padding:0 8px 10px;
    }

    thead th{
        font-size:13px;
    }

    tbody td{
        height:47px;
    }

    .rank{
        font-size:18px;
    }

    .name-box{
        width:94%;
        height:32px;
    }

    .name-box input{
        font-size:11px;
    }

    .points-box{
        width:55px;
        height:32px;
    }

    .points-box input{
        font-size:17px;
    }

    .info{
        width:94%;
        grid-template-columns:1fr 1fr;
        padding:8px;
    }

    .info-item{
        min-height:78px;
        justify-content:flex-start;
        padding:8px;
        border-bottom:1px solid rgba(225,173,35,.4);
    }

    .info-item:nth-child(2),
    .info-item:nth-child(4){
        border-right:0;
    }

    .info-item:nth-child(3),
    .info-item:nth-child(4){
        border-bottom:0;
    }

    .info-icon{
        font-size:25px;
    }

    .info-label{
        font-size:9px;
    }

    .info-value{
        font-size:12px;
    }

    .quote{
        font-size:14px;
    }
}

</style>
</head>

<body>

<header class="header">

    <div class="logo-name">
        <span class="trophy">🏆</span>
        LYRICS VIBES TEAM
    </div>

    <div class="menu">
        <i></i>
        <i></i>
        <i></i>
    </div>

</header>


<main class="main">

    <div class="microphone">
        <div class="mic-body"></div>
        <div class="mic-line"></div>
        <div class="mic-neck"></div>
        <div class="mic-base"></div>
    </div>


    <div class="laurel">❯</div>
    <div class="laurel right">❯</div>


    <div class="lvt">
        LVT
    </div>


    <h1 class="competition-title">
        LYRICS COMPETITION
    </h1>


    <div class="date">
        5/9/2026
    </div>


    <div class="stars">
        — ★ ★ ★ ★ ★ —
    </div>


    <p class="description">
        A platform to showcase creativity, talent and<br>
        passion for lyrics.
    </p>


    <div class="live-box">
        <span class="live-circle"></span>
        LIVE COMPETITION
    </div>


    <section class="table-card">

        <div class="table-wrap">

            <table>

                <thead>
                    <tr>
                        <th>RANK</th>
                        <th>CONTESTANT</th>
                        <th>POINTS</th>
                    </tr>
                </thead>

                <tbody id="contestants"></tbody>

            </table>

        </div>

    </section>


    <section class="info">

        <div class="info-item">
            <div class="info-icon">📅</div>

            <div>
                <div class="info-label">DATE</div>
                <div class="info-value">5/9/2026</div>
            </div>
        </div>


        <div class="info-item">
            <div class="info-icon">◷</div>

            <div>
                <div class="info-label">STATUS</div>
                <div class="info-value">LIVE NOW</div>
            </div>
        </div>


        <div class="info-item">
            <div class="info-icon">🏆</div>

            <div>
                <div class="info-label">TOTAL CONTESTANTS</div>
                <div class="info-value">16</div>
            </div>
        </div>


        <div class="info-item">
            <div class="info-icon">🎁</div>

            <div>
                <div class="info-label">WINNER REWARD</div>
                <div class="info-value">
                    Exciting Prizes<br>
                    & Recognition
                </div>
            </div>
        </div>

    </section>


    <p class="quote">
        “Creativity is intelligence having fun. Let your lyrics speak and inspire the world.”
    </p>

</main>


<script>

const contestants = document.getElementById("contestants");

for(let i = 1; i <= 16; i++){

    contestants.innerHTML += `
        <tr>

            <td class="rank">
                ${i}
            </td>

            <td>
                <div class="name-box">
                    <input
                        type="text"
                        aria-label="Contestant ${i}"
                    >
                </div>
            </td>

            <td>
                <div class="points-box">
                    <input
                        type="text"
                        value="-"
                        aria-label="Points ${i}"
                    >
                </div>
            </td>

        </tr>
    `;

}

</script>

</body>
</html>