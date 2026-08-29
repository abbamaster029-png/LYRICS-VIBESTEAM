<section class="results-section">

    <div class="section-title">
        🏆 OFFICIAL FINAL RESULTS
    </div>

    <div class="results-table">

        <div class="result-row result-head">
            <div>RANK</div>
            <div>PARTICIPANT</div>
            <div>POINTS</div>
            <div>RECOGNITION</div>
        </div>

        <div class="result-row">
            <div>🥇 1</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>🥈 2</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>🥉 3</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>🏅 4</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>5</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>6</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>7</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>8</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>9</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>10</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>11</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>12</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>13</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>14</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>15</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

        <div class="result-row">
            <div>16</div>
            <div></div>
            <div></div>
            <div></div>
        </div>

    </div>

</section>

<style>

.results-section{
    width:94%;
    max-width:900px;
    margin:25px auto;
    padding:15px;
    border:1px solid #c99b24;
    border-radius:13px;
    background:#061d3b;
}

.section-title{
    margin-bottom:16px;
    color:#f1b82c;
    font-family:"Inter",Arial,sans-serif;
    font-size:19px;
    font-weight:800;
}

.results-table{
    width:100%;
    overflow:hidden;
    border:1px solid #315075;
}

.result-row{
    display:grid;
    grid-template-columns:14% 42% 17% 27%;
    min-height:38px;
    align-items:center;
    border-bottom:1px solid rgba(80,112,145,.28);
    color:#e8edf4;
    font-family:"Inter",Arial,sans-serif;
    font-size:11px;
}

.result-row:last-child{
    border-bottom:0;
}

.result-row > div{
    min-height:38px;
    padding:8px;
    display:flex;
    align-items:center;
    border-right:1px solid rgba(80,112,145,.22);
}

.result-row > div:last-child{
    border-right:0;
}

.result-head{
    min-height:33px;
    background:#071c38;
    color:#dce5ef;
    font-size:10px;
    font-weight:800;
}

.result-head > div{
    min-height:33px;
}

.result-row:not(.result-head):nth-child(even){
    background:rgba(7,31,57,.55);
}

@media(max-width:600px){

    .results-section{
        width:96%;
        padding:11px;
        margin:20px auto;
    }

    .section-title{
        font-size:16px;
        margin-bottom:12px;
    }

    .result-row{
        grid-template-columns:13% 39% 17% 31%;
        min-height:34px;
        font-size:9px;
    }

    .result-row > div{
        min-height:34px;
        padding:6px 5px;
    }

    .result-head{
        min-height:30px;
        font-size:8px;
    }

    .result-head > div{
        min-height:30px;
    }
}

</style>