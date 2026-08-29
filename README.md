<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#03152d">

<title>LVT | Live Competition</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&family=Playfair+Display:wght@700;800&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    min-height:100vh;
    overflow-x:hidden;
    font-family:"Inter",sans-serif;
    color:#fff;
    background:
        radial-gradient(circle at 50% 10%,#073a82 0%,#032352 35%,#03152d 72%);
}

/* HEADER */

.header{
    height:58px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    padding:0 18px;
    background:#08090c;
    border-bottom:1px solid #e5ad27;
}

.brand{
    display:flex;
    align-items:center;
    gap:8px;
    color:#f2b52b;
    font-size:18px;
    font-weight:800;
}

.brand span{
    font-size:22px;
}

.menu{
    width:42px;
    height:38px;
    border:1px solid #dca51e;
    border-radius:8px;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    gap:5px;
}

.menu i{
    width:23px;
    height:2px;
    background:#eab32a;
}

/* MAIN */

.main{
    width:100%;
    max-width:950px;
    margin:auto;
    padding:25px 16px 28px;
    position:relative;
}

/* LVT */

.lvt{
    text-align:center;
    font-family:"Playfair Display",serif;
    font-size:clamp(70px,12vw,115px);
    line-height:.85;
    letter-spacing:3px;
    color:#f5bd35;
    text-shadow:
        0 2px 0 #805400,
        0 0 16px rgba(255,190,40,.45);
}

.title{
    text-align:center;
    margin-top:8px;
    font-family:"Playfair Display",serif;
    font-size:clamp(27px,4vw,43px);
    color:#f2b82d;
    line-height:1;
}

/* DATE */

.date{
    width:max-content;
    margin:14px auto 0;
    padding:6px 28px;
    border:1px solid #e7ad25;
    border-radius:9px;
    color:#f3b62c;
    font-size:25px;
    font-weight:800;
}

/* STARS */

.stars{
    text-align:center;
    margin:8px 0 12px;
    color:#f1b62b;
    font-size:21px;
    letter-spacing:4px;
}

.description{
    text-align:center;
    font-size:16px;
    line-height:1.45;
}

/* LIVE */

.live-box{
    width:min(450px,90%);
    margin:20px auto -1px;
    padding:7px 15px;
    text-align:center;
    color:#f2b62b;
    font-size:18px;
    font-weight:800;
    border:1px solid #e5ac25;
    border-radius:14px;
    background:#06234b;
    position:relative;
    z-index:3;
}

.live-dot{
    display:inline-block;
    width:15px;
    height:15px;
    margin-right:7px;
    vertical-align:-2px;
    background:#f2b52b;
    border-radius:50%;
}

/* TABLE */

.table-card{
    width:92%;
    margin:auto;
    padding:0 13px 13px;
    border:1.5px solid #dda91e;
    border-radius:13px;
    background:rgba(2,22,49,.84);
}

.table-wrap{
    overflow:hidden;
    border:1px solid #e3ad25;
    border-radius:11px;
}

table{
    width:100%;
    border-collapse:collapse;
    table-layout:fixed;
}

thead th{
    height:40px;
    color:#efb62a;
    font-size:14px;
    font-weight:700;
    border-bottom:1px solid #d9a21c;
}

thead th:first-child{
    width:14%;
}

thead th:last-child{
    width:18%;
}

tbody td{
    height:43px;
    text-align:center;
    border-right:1px solid rgba(221,174,45,.25);
    border-bottom:1px solid rgba(221,174,45,.25);
}

tbody tr:last-child td{
    border-bottom:0;
}

tbody td:last-child{
    border-right:0;
}

.rank{
    color:#f0b62a;
    font-size:17px;
    font-weight:800;
}

/* LIST STYLE LIKE THE IMAGE */

.contestant{
    width:88%;
    height:32px;
    margin:auto;
    border:1px solid rgba(158,171,191,.55);
    border-radius:7px;
    background:rgba(2,14,31,.65);
    display:flex;
    align-items:center;
    padding:0 8px;
}

.contestant input{
    width:100%;
    border:0;
    outline:0;
    background:transparent;
    color:#fff;
    text-align:center;
    font-family:"Inter",sans-serif;
    font-size:12px;
}

.points{
    color:#f2b72c;
    font-size:16px;
    font-weight:700;
}

/* INFO BAR */

.info{
    width:92%;
    margin:14px auto 0;
    padding:13px 14px;
    border:1.5px solid #dfa820;
    border-radius:11px;
    background:rgba(3,24,50,.88);
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.info-item{
    min-height:52px;
    display:flex;
    align-items:center;
    justify-content:center;
    gap:8px;
    border-right:1px solid rgba(225,173,35,.5);
}

.info-item:last-child{
    border-right:0;
}

.icon{
    font-size:23px;
}

.label{
    color:#f0b62b;
    font-size:9px;
    font-weight:700;
    margin-bottom:3px;
}

.value{
    font-size:12px;
    line-height:1.25;
}

/* QUOTE */

.quote{
    width:90%;
    margin:17px auto 0;
    text-align:center;
    color:#e9ae28;
    font-size:13px;
    font-style:italic;
    line-height:1.4;
}

/* MOBILE */

@media(max-width:600px){

    .header{
        height:56px;
        padding:0 13px;
    }

    .brand{
        font-size:15px;
    }

    .brand span{
        font-size:20px;
    }

    .main{
        padding:22px 5px 25px;
    }

    .lvt{
        font-size:78px;
    }

    .title{
        font-size:27px;
    }

    .date{
        font-size:22px;
        padding:5px 22px;
    }

    .stars{
        font-size:19px;
    }

    .description{
        font-size:14px;
    }

    .live-box{
        font-size:16px;
        width:86%;
    }

    .table-card{
        width:96%;
        padding:0 7px 8px;
    }

    thead th{
        height:37px;
        font-size:12px;
    }

    tbody td{
        height:40px;
    }

    .rank{
        font-size:15px;
    }

    .contestant{
        width:94%;
        height:29px;
    }

    .contestant input{
        font-size:10px;
    }

    .points{
        font-size:14px;
    }

    .info{
        width:96%;
        grid-template-columns:1fr 1fr;
        padding:5px;
    }

    .info-item{
        min-height:58px;
        justify-content:flex-start;
        padding:6px;
        border-bottom:1px solid rgba(225,173,35,.35);
    }

    .info-item:nth-child(2),
    .info-item:nth-child(4){
        border-right:0;
    }

    .info-item:nth-child(3),
    .info-item:nth-child(4){
        border-bottom:0;
    }

    .icon{
        font-size:20px;
    }

    .label{
        font-size:8px;
    }

    .value{
        font-size:10px;
    }

    .quote{
        font-size:12px;
    }
}
</style>
</head>

<body>

<header class="header">

    <div class="brand">
        <span>🏆</span>
        LYRICS VIBES TEAM
    </div>

    <div class="menu">
        <i></i>
        <i></i>
        <i></i>
    </div>

</header>


<main class="main">

    <div class="lvt">LVT</div>

    <h1 class="title">
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
        <span class="live-dot"></span>
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
            <div class="icon">📅</div>
            <div>
                <div class="label">DATE</div>
                <div class="value">5/9/2026</div>
            </div>
        </div>


        <div class="info-item">
            <div class="icon">◷</div>
            <div>
                <div class="label">STATUS</div>
                <div class="value">LIVE NOW</div>
            </div>
        </div>


        <div class="info-item">
            <div class="icon">🏆</div>
            <div>
                <div class="label">TOTAL CONTESTANTS</div>
                <div class="value">16</div>
            </div>
        </div>


        <div class="info-item">
            <div class="icon">🎁</div>
            <div>
                <div class="label">WINNER REWARD</div>
                <div class="value">
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

    const row = document.createElement("tr");

    row.innerHTML = `
        <td class="rank">${i}</td>

        <td>
            <div class="contestant">
                <input type="text">
            </div>
        </td>

        <td class="points">-</td>
    `;

    contestants.appendChild(row);
}

</script>

</body>
</html>