<template>
  <div id="home">
    <div className="home container">
      <div className="title">
        <WeatherIcon />
        <h2 class="main-title">Weather App</h2>
      </div>
      <div className="search">
        <input type="text" placeholder="Enter a city">
        <button>Search</button>
      </div>
    </div>
  </div>
</template>
  
<style>
*{
    padding: 0;
    margin: 0;
    font-family: Arial, Helvetica, sans-serif;
}
.container {
  min-height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
#home {
	background-image: url(../assets/vue-js-kk.jpg);
	background-size: cover;
	background-position: top center;
	position: relative;
	z-index: 1;
}
#home::after {
	content: '';
	position: absolute;
	left: 0;
	top: 0;
	height: 100%;
	width: 100%;
	background-color: black;
	opacity: 0.3;
	z-index: -1;
}
#home .home {
	max-width: 1200px;
	margin: 0 auto;
	padding: 0 auto;
    align-items: center;
	justify-content: center;
}
.home{
    color: white;
    display: flex;
    flex-direction: column;
}
.title{
    padding: 20px 0;
	display: flex;
	flex-direction: row;
	align-items: center;
	justify-content: center;
	gap: 10px;
}
.main-title{
    font-size: 2em;
    text-transform: uppercase;
}
input{
    color: white;
    background-color: black;
    padding: 10px;
    font-size: 16px;
    border: none;
    border-radius: 4px;
}
button{
    padding: 10px;
    font-size: 16px;
    color: white;
    background-color: rgb(12, 145, 56);
    border: none;
    border-radius: 4px;
    cursor: pointer;
}
/* @media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
} */
</style>
  