<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#03152d">

<title>LYRICS VIBES TEAM | Live Competition</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Playfair+Display:wght@700;800&display=swap" rel="stylesheet">

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

body{
    min-height:100vh;
    overflow-x:hidden;
    font-family:Inter,Arial,sans-serif;
    color:#fff;
    background:
        radial-gradient(circle at 50% 15%,rgba(0,90,255,.28),transparent 35%),
        radial-gradient(circle at 10% 40%,rgba(0,80,190,.20),transparent 30%),
        #03152d;
}

/* HEADER */
.header{
    height:68px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:0 28px;
    background:#08090d;
    border-bottom:2px solid #e2aa22;
}

.brand{
    display:flex;
    align-items:center;
    gap:12px;
    color:#f2b72c;
    font-size:24px;
    font-weight:800;
}

.brand-icon{
    font-size:29px;
}

.menu{
    width:50px;
    height:46px;
    border:1px solid #e1aa25;
    border-radius:10px;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    gap:6px;
}

.menu span{
    width:28px;
    height:2px;
    background:#eab32c;
}

/* HERO */
.hero{
    text-align:center;
    padding:38px 20px 15px;
}

.logo{
    font-family:"Playfair Display",serif;
    font-size:clamp(75px,15vw,140px);
    line-height:.9;
    letter-spacing:5px;
    color:#f5ba2d;
    text-shadow:
        0 2px 0 #8b5b00,
        0 0 18px rgba(255,194,40,.55);
}

.title{
    margin-top:8px;
    font-family:"Playfair Display",serif;
    font-size:clamp(28px,5vw,55px);
    color:#f2b72b;
}

.date{
    display:inline-block;
    margin-top:17px;
    padding:8px 38px;
    border:1px solid #efb32a;
    border-radius:11px;
    color:#f4bb31;
    font-size:clamp(24px,4vw,38px);
    font-weight:800;
}

.stars{
    margin:10px 0 15px;
    color:#f4b82d;
    font-size:25px;
    letter-spacing:5px;
}

.description{
    max-width:650px;
    margin:auto;
    font-size:19px;
    line-height:1.55;
}

/* LIVE TITLE */
.live-title{
    width:min(500px,88%);
    margin:27px auto 0;
    padding:9px 20px;
    text-align:center;
    border:1px solid #e9ae25;
    border-radius:17px;
    background:rgba(4,25,54,.85);
    color:#f2b62b;
    font-size:23px;
    font-weight:800;
}

.live-dot{
    display:inline-block;
    width:20px;
    height:20px;
    margin-right:9px;
    vertical-align:-2px;
    border-radius:50%;
    background:#f3b52a;
    box-shadow:0 0 12px rgba(243,181,42,.7);
}

/* TABLE */
.board{
    width:min(960px,88%);
    margin:auto;
    padding:0 18px 17px;
    border:2px solid #dfa820;
    border-radius:15px;
    background:rgba(4,28,59,.82);
}

.table-wrap{
    overflow:hidden;
    border:1px solid #e2ac24;
    border-radius:14px;
}

table{
    width:100%;
    border-collapse:collapse;
    table-layout:fixed;
}

thead th{
    height:48px;
    color:#efb62b;
    font-size:18px;
    border-bottom:1px solid #d89f1b;
}

thead th:first-child{
    width:14%;
}

thead th:last-child{
    width:19%;
}

tbody td{
    height:52px;
    text-align:center;
    border-right:1px solid rgba(211,169,52,.25);
    border-bottom:1px solid rgba(211,169,52,.28);
}

tbody tr:last-child td{
    border-bottom:0;
}

tbody td:last-child{
    border-right:0;
}

.rank{
    color:#f2b92d;
    font-size:23px;
    font-weight:800;
}

.name-cell{
    padding:7px 18px;
}

.name-input,
.points-input{
    width:100%;
    height:36px;
    outline:none;
    border:1px solid rgba(176,186,202,.5);
    border-radius:8px;
    background:rgba(2,15,31,.65);
    color:#fff;
    text-align:center;
}

.name-input:focus,
.points-input:focus{
    border-color:#eab32b;
}

.points-input{
    max-width:75px;
}

/* INFO */
.info{
    width:min(960px,88%);
    margin:16px auto 0;
    padding:20px 22px;
    border:2px solid #dfa820;
    border-radius:13px;
    background:rgba(4,25,51,.82);
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.info-item{
    min-height:66px;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:12px;
    border-right:1px solid rgba(221,171,34,.55);
}

.info-item:last-child{
    border-right:0;
}

.info-icon{
    font-size:32px;
}

.info-label{
    margin-bottom:5px;
    color:#f0b62b;
    font-size:13px;
    font-weight:700;
}

.info-value{
    font-size:16px;
}

.quote{
    width:90%;
    margin:22px auto 35px;
    text-align:center;
    color:#eab32c;
    font-size:16px;
    font-style:italic;
    line-height:1.5;
}

/* MOBILE */
@media(max-width:700px){

    .header{
        height:64px;
        padding:0 15px;
    }

    .brand{
        font-size:17px;
        gap:7px;
    }

    .brand-icon{
        font-size:23px;
    }

    .menu{
        width:46px;
        height:42px;
    }

    .hero{
        padding-top:27px;
    }

    .date{
        padding:7px 25px;
    }

    .description{
        font-size:16px;
    }

    .board,
    .info{
        width:94%;
    }

    .board{
        padding:0 8px 10px;
    }

    thead th{
        font-size:14px;
    }

    tbody td{
        height:47px;
    }

    .rank{
        font-size:18px;
    }

    .name-cell{
        padding:6px 5px;
    }

    .name-input{
        height:33px;
        font-size:12px;
    }

    .points-input{
        height:33px;
        max-width:58px;
        font-size:13px;
    }

    .info{
        grid-template-columns:1fr 1fr;
        padding:8px;
    }

    .info-item{
        min-height:76px;
        justify-content:flex-start;
        padding:8px 10px;
        border-bottom:1px solid rgba(221,171,34,.4);
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
        font-size:10px;
    }

    .info-value{
        font-size:13px;
    }
}
</style>
</head>

<body>

<header class="header">
    <div class="brand">
        <span class="brand-icon">🏆</span>
        LYRICS VIBES TEAM
    </div>

    <div class="menu">
        <span></span>
        <span></span>
        <span></span>
    </div>
</header>

<section class="hero">

    <div class="logo">LVT</div>

    <h1 class="title">LYRICS COMPETITION</h1>

    <div class="date">5/9/2026</div>

    <div class="stars">
        — ★ ★ ★ ★ ★ —
    </div>

    <p class="description">
        A platform to showcase creativity, talent and<br>
        passion for lyrics.
    </p>

</section>

<div class="live-title">
    <span class="live-dot"></span>
    LIVE COMPETITION
</div>

<section class="board">

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

<script>

const contestants = document.getElementById("contestants");

for(let i = 1; i <= 16; i++){

    const row = document.createElement("tr");

    row.innerHTML = `
        <td class="rank">${i}</td>

        <td class="name-cell">
            <input
                class="name-input"
                type="text"
                aria-label="Contestant ${i}"
            >
        </td>

        <td>
            <input
                class="points-input"
                type="text"
                value="-"
                aria-label="Points ${i}"
            >
        </td>
    `;

    contestants.appendChild(row);
}

</script>

</body>
</html>