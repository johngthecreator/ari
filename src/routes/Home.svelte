<script>
</script>
<main>
    <div id="heroBanner">
        <img src="sitting.webp" alt="person sitting"/>
        <h1>Math Made Simple.</h1>
    </div>
    <div class="infoContainer">
        <div class="infoText">
            <h2>What Is Ari?</h2>
            <p>Ari is an innovative web application that utilizes short and engaging games to reinforce mathematical concepts. It helps users solidify their understanding of mathematical principles in a fun and interactive way, making the learning process enjoyable and memorable. Whether you're a student looking to improve your math skills or an educator searching for a fresh and engaging way to teach, Ari is the perfect tool for you. With its focus on practical application and interactive gameplay, Ari is changing the way people think about mathematics and learning.</p>
        </div>
        <img class="infoImg" src="https://images.unsplash.com/photo-1509062522246-3755977927d7?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=500&q=80" alt="person sitting"/>
    </div>
    <div class="infoContainer">
        <img class="infoImg" src="https://images.unsplash.com/photo-1532356884227-66d7c0e9e4c2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1770&q=80" alt="person sitting"/>
        <div class="infoText">
            <h2>Learn On The Go</h2>
            <p>Ari is designed to fit the fast-paced and demanding environments we live and work in. The short and engaging games are carefully crafted to make the most of limited time, providing quick and effective learning sessions that can be easily integrated into a busy schedule. Whether you're on a break at work or commuting to school, Ari provides the flexibility and convenience needed to keep up with the demands of modern life. With its efficient approach to learning, Ari is the perfect solution for anyone looking to improve their mathematical understanding in today's fast-paced world.</p>
        </div>
    </div>
</main>
<style>
    div#heroBanner{
        background-color: #BCB6FF;
        text-align: center;
        padding: 15px;
    }
    #heroBanner h1 {
        color: white;
    }
    div.infoText {
        padding: 20px;
        width: 50%;
    }
    div.infoContainer {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        margin-top: 100px;
    }
    img.infoImg {
        width: 50%;
        margin: 15px;
        border-radius: 10px;
        border: 5px solid #BCB6FF;
    }
    @media screen and (max-width: 768px){
        div.infoContainer {
            display: flex;
            flex-direction: column;
            justify-content: none;
        }
        div.infoText {
        width: 100%;
        }
        img.infoImg {
            width: 100%;
            margin: 0;
            margin-bottom: 10px;
            border-radius: 10px;
            border: 5px solid #BCB6FF;
        }

    }

</style>