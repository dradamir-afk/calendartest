<template>
    <div class="container">
        <div class="calendar">
            <div class="month">
                <i class="fas fa-angle-left prev"></i>
                <div class="date">
                    <h1>Year</h1>
                    <p>Month</p>
                </div>
                <i class="fas fa-angle-right next"></i>
            </div>
            <div class="weekdays">
                <div>Вс</div>
                <div>Пнд</div>
                <div>Вт</div>
                <div>Ср</div>
                <div>Чт</div>
                <div>Пт</div>
                <div>Сб</div>
            </div>
            <div class="days">
                <div class="prev-date">26</div>
                <div class="prev-date">27</div>
                <div class="prev-date">28</div>
                <div class="prev-date">29</div>
                <div class="prev-date">30</div>
                <div>1</div>
                <div>2</div>
                <div>3</div>
                <div>4</div>
                <div>5</div>
                <div>6</div>
                <div>7</div>
                <div>8</div>
                <div>9</div>
                <div>10</div>
                <div>11</div>
                <div>12</div>
                <div>13</div>
                <div>14</div>
                <div>15</div>
                <div>16</div>
                <div>17</div>
                <div>18</div>
                <div>19</div>
                <div>20</div>
                <div>21</div>
                <div>22</div>
                <div>23</div>
                <div>14</div>
                <div>25</div>
                <div>26</div>
                <div>27</div>
                <div>28</div>
                <div class="today">29</div>
                <div>30</div>
                <div>31</div>
                <div class="next-date">1</div>
                <div class="next-date">2</div>
                <div class="next-date">3</div>
                <div class="next-date">4</div>
                <div class="next-date">5</div>
                <div class="next-date">6</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
*{
    margin:0;
    padding:0;
    box-sizing: border-box;
    /* font-family: 'Quicksand', sans-serif; */
}
html{
    font-size: 10%;
}
.container{
    width: 100%;
    min-height:100vh;
    background-color: #12121f;
    color:#eee;
    display: flex;
    justify-content: center;
    align-items: center;
}
.calendar{
    width: 45rem;
    /* height: 52rem; */
    background-color: #222227;
    box-shadow: 0.5rem 3rem rgba(0,0,0,0.4);
}
.month{
    width: 100%;
    height: 12rem;
    background-color: #167e56;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding:0 2rem;
    text-align: center;
    text-shadow: 0 0.3rem 0.5rem rgba(0, 0, 0, 0.5);
}
.month i{
    font-size: 2.5rem;
    cursor: pointer;
}

.month h1{
    font-size: 3rem;
    font-weight: 400;
    text-transform: uppercase;
    letter-spacing: 0.2rem;
    margin-bottom: 1rem;
}

.month p{
    font-size: 1.6rem;
}

.weekdays{
    width: 100%;
    height: 5rem;
    padding: 0 0.4rem;
    display: flex;
    align-items: center;
}

.weekdays div{
    font-size: 1.5rem;
    font-weight: 400;
    letter-spacing: 0.1rem;
    width: calc(44.2rem/7);
    display: flex;
    justify-content: center;
    align-items: center;
    text-shadow:0 0.3rem 0.5rem rgba(0, 0, 0, 0.5);
}

.days{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
    padding: 0.2rem;
}

.days div{
    font-size: 1.4rem;
    margin: 0.3rem;
    width: calc(40.2rem / 7);
    height: 5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    /* transition: background-color 0.7s; */
}

.prev-date,.next-date{
    opacity: 0.5;
}

.days div:hover:not(.today){
    background-color: #262626;
    border: 2px solid #777;
    cursor: pointer;
}

.days div:hover{
    border:2px solid white;
    cursor: pointer;
}

.today{
    background-color: #167e56;
}

</style>