# Zomato-CLONE-landing-page-CSS-
CSS Code




*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

.hero__section{
    background: url(./images/heroSectionBackground.png);
    background: url(images/heroSectionBackground.png);
    background-size: cover;
    background-position: center;
    color: white;
    min-height: 60vh;
}
.navbar{
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 65px;
    padding: 16px 48px;
}
.navbar a{
    color: white;
    text-decoration: none;
}
.navbar__menu_container{
    display: flex;
    gap: 18px;
    /* padding-right: 18px; */
}
.navbar__menu_container .user_icon{
    height: 25px;
    width: 25px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 100%;
    border: solid 1px white;
    display: none;
}
.hero__section_container{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 20px;
    height: calc(60vh - 65px);
    
}
.hero__section_logo{
    width: 200px;
    height: 40px;
    /* height: auto; */
}
.hero__section_title{
    text-align: center;
    font-size: 30px;
    font-weight: 380;
}
.hero__section_input_container{
    background-color: white;
    padding: 10px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    width: 50%;
    border-radius: 10px;
}
.input_container_location, 
.input_container_search{
    padding: 5px;
    border: none;
    outline: none;
}
.input_container_location{
    width: 35%;
    border-right: 2px solid #e0e0e0;
}
.input_container_search{
    width: 65%;
}
/* Screen Size is from 0-600 i.e., smaller/mobile screen */
@media only screen and (max-width: 600px){
    .navbar__menu_container .user_icon{
        display: flex;
    }
    .link{
        display: none;
    }
    .hero__section{
        min-height: 80vh;
    }
    .hero__section_container{
        flex-direction: column;
        background-color: transparent;
        width: 100%;
    }
    .input_container_location,
    .input_container_search{
        padding: 18px;
        border-radius: 10px;
        width: 98%;
    }
    .hero__section_container{
        height: calc(80vh - 40px);
    }
    .hero__section_title{
        font-size: 18px;
        width: 95%;
    }
}
/* Out of media queries */
.container{
    margin: 3rem auto;
    width: 90%;
}
.we__offer{
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
    align-items: center;
    justify-content: center;
}
.we__offer_card{
    border-radius: 10px;
    /* background-color: aqua; */
    overflow: hidden;
    border: 1px solid #e0e0e0;
    transition: all 1s ease;
    margin-right: 12px;
}
.we__offer_card:hover{
    transform: scale(1.1);
}
.we__offer_card img{
    width: 100%;
    height: 170px;
    object-fit: cover;
    object-position: center;
}
.we__offer_content{
    padding: 10px;
}
.we__offer_content h2{
    font-size: 20px;
    font-weight: 400;
}
.we__offer_content p{
    font-size: 12.5px;
}
.collections h1{
    font-weight: 600;
}
.collections .sub__heading_container{
    font-size: 15px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 1rem;
}
.sub__heading_container span:nth-child(2){
    color: #ff7e8b;
    font-size: 13px;
    cursor: pointer;
}
.collections_card_container{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    gap: 0.5rem;
    margin-top: 1.25rem;
}
.collections_card_container .card{
    height: 300px;
    min-width: 240px;
    background-size: cover;
    background-position: center;
    border-radius: 10px;
    position: relative;
}

.card1{
    background-image: url('./images/collection1.jpg');
    background-image: url('images/collection1.jpg');
}

.card2{
    background-image: url('./images/collection2.jpg');
    background-image: url('images/collection2.jpg');
}

.card3{
    background-image: url('./images/collection3.jpg');
    background-image: url('images/collection3.jpg');
}

.card4{
    background-image: url('./images/collection4.jpg');
    background-image: url('images/collection4.jpg');
}

/* rgba => Red, Green, Blue, Opacity */
.overlay{
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    border-radius: 10px;
    background: linear-gradient(
      
        rgba(225, 0, 0, 1) 0%,
        rgba(225, 0, 2, 1) 50%,
        rgba(225, 0, 0, 1) 85%,
    );
    z-index: 5;
}
.collections_card_container .card .content{
    position: absolute;
    bottom: 0;
    left: 0;
    color: white;
    padding: 12px 16px;
    font-size: 0.9rem;
    z-index: 6;
}
.content h4{
    font-weight: 400;
    letter-spacing: 0.5px;
}
.get__the_app{
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgb(255,251,247);
    width: 100%;
    padding: 3rem 6rem;
}
.get__the_app .semiContainer{
    width: 60%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 1.5rem;
}
.get__the_app .semiContainer .left{
    flex: 2;
}
.get__the_app .semiContainer .left img{
    width: 100%;
    object-fit: cover;
    object-position: center;
}
.get__the_app .semiContainer .right{
    flex: 3;
    height: 100%;
    display: flex;
    flex-direction: column;
    gap: 1rem;
}
.right h1{
    font-weight: 400;
    font-size: 2rem;
}
.right p{
    font-size: 0.8rem;
}
.right .radio__button_container{
    display: flex;
    align-items: center;
    gap: 1rem;
}
.right .radio__button_container div{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
}
.right .radio__button_container div input{
    height: 15px;
    width: 15px;
    accent-color: rgb(239, 79, 95);
}
.right .input_container{
    display: flex;
    gap: 0.5rem;
}
.input_container{
    flex-wrap: wrap;
}
.input_container button,
.input_container input{
    padding: 10px 12px;
}
.input_container input{
    flex: auto;
    border:  1.5px solid gray;
    outline: none;
    border-radius: 5px;
}
.input_container button{
    border: none;
    background-color: rgb(239, 79, 95);
    color: white;
    border-radius: 5px;
    cursor: pointer;
}
.right .download__app_container{
    display: flex;
    flex-direction: column;
    gap: 0.7rem;
}
.right .download__app_container h5{
    font-weight: 400;
    color: gray;
}
.right .download__app_container div{
    display: flex;
    gap: 1rem;
}
.right .download__app_container div img{
    width: 35%;
}
/* Media Queries For Download App */
/* 0-1300 */
@media only screen and (max-width: 1300px){
    .get__the_app .semiContainer .left,
    .get__the_app .semiContainer .right{
        flex: 1;
    }
    .get__the_app .semiContainer{
        width: 80%;
    }
}
/* 0-900 */
@media only screen and (max-width: 900px){
    .get__the_app{
        padding: 2rem 0;
    }
    .get__the_app .semiContainer{
        width: 95%;
        flex-direction: column;
    }
}
.footer{
    width: 100%;
}
.footer_section1{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    width: 80%;
    margin: auto;
}
.footer_section1 img{
    width: 130px;
}
.section1__buttonContainer{
    display: flex;
    gap: 1rem;
}
.section1__buttonContainer button{
    padding: 5px;
    width: 90px;
    border: 1px solid gray;
    border-radius: 5px;
    background-color: transparent;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 12px;
    cursor: pointer;
}
.navigation_container{
    display: grid;
    /* grid-template-columns: 1fr 1fr 1fr 1fr 1fr; */
    grid-template-columns: repeat(5, 1fr);
    width: 80%;
    margin: auto;
    gap: 1rem;
    padding: 3rem 0;
}
.link__container{
    display: flex;
    flex-direction: column;
    gap: 5px;
}
.link__container h5{
    font-weight: 500;
    font-size: 15px;
    margin-bottom: 5px;
    letter-spacing: 0.8px;
}
.footer__link{
    text-decoration: none;
    color: gray;
    font-size: 12.5px;
    font-weight: 300;
}
.footer__link:hover{
    color: black;
}
.section__links_container button{
  background-color: black;
  border: none;
  width: 25px;
  height: 25px;
  border-radius: 30px;
  color: white;
  cursor: pointer;
}
.section__links_container button i{
    /* color: white; */
    font-size: 13px;
    display: flex;
    /* horizontal / x-axis */
    align-items: center; 
    /* Vertical / y-axis */
    justify-content: center;
}
.footer__section_logos{
    width: 100%;
}
.disclamer{
    width: 95%;
    color: gray;
    margin: auto;
    border-top: 1px solid gray;
    padding-top: 1.5rem;
}
@media only screen and (max-width: 900px){
    .navigation_container{
            grid-template-columns: repeat(3, 1fr);
    }
}
@media only screen and (max-width: 500px){
    .navigation_container{
            grid-template-columns: repeat(2, 1fr);
    }
}
@media only screen and (max-width: 320px){
    .navigation_container{
            grid-template-columns: repeat(1, 1fr);
    }
}


