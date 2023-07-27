THIS IS MY ORIGINAL CSS FILE INCASE YOU NEED IT AGAIN

```CSS
* {
    box-sizing: border-box;
    background-color: #E4E5E7;
  }

/* layout test with css coder */
.wrapper {
  display: flex;
  flex-flow: row wrap;
  text-align: center;
}

.wrapper > * {
  padding: 10px;
  margin: 10px;
  flex: 1 100%;
  border-radius: 10px;
}

.header {
  height: 120px;
}

.main { 
  height: 300px;
}

@media all and (min-width: 800px){
  .main{
    flex: 3;
  }

  .aside{
    order: 1;
  }
}

@media all and (min-width: 600px){
  .aside{
    flex: 1;
  }
}

/* HEADER.JSX */

.header {
    display: flex;
    align-items: center;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.15);
}

.header--logo {
    width: 50px; 
    margin-left: 20px;
    margin-bottom: 10px;
}

.header--title {
    flex: 1;
    text-align: center;
    margin-right: 120px;
    color: rgb(0, 0, 0);
    font-family: 'Plus Jakarta Sans', sans-serif;
}

.search--bar {
  position: absolute;
  top: 23px;
  right:170px;
  font-size: 22px;
  border-radius: 20px;
  padding: 0.5%;
  padding-left: 15px;
  background: url(./search-icon-png)
}

.search--bar--button {
  position: absolute;
  top: 32px;
  right: 130px;
}

/* MAIN.JSX */

/* recommendations */
.recommendations--title {
 font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
 font-size: 40px;
 margin-bottom: 0px;
}

.recommendations--subtitle {
  font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
  color: #918E9B;
  margin-top: 0px;

}

/* sort by */
.sorting--options {
  display: flex;
  align-items: center;

}

/*  for previews */
.podcast-previews {
    display: flex;
    flex-wrap: wrap;
  }
  
  .podcast-preview {
    width: 300px;
    margin: 10px;
    padding: 10px;
  }
  
  .podcast-preview h2 {
    font-size: 18px;
    margin-bottom: 5px;
  }
  
  .podcast-preview img {
    width: 100%;
    height: auto;
    margin-bottom: 5px;
    border-radius: 30px
  }

  .podcast--image:hover {
    filter: brightness(50%);
  }
  
  .podcast-preview p {
    font-size: 14px;
  }

.open--preview--button {
  /* width: 50px; this doesnt work for some reason. it only works if you move the img to under the h1 "this is working" */
  max-width: 30%;
  /* 1 */
  position: absolute;
  top: 180px;
  left: 180px;
}

.open--preview--button:hover {
  max-width: 40%;
}

.favorite--icon {
  max-width: 12%;
  position: absolute;
  top: 300px;
  left: 250px;
}

.preview--image {
  position: relative;
  top: 0;
  left: 0;
}

.podcast--image {
  position: relative;
  top: 0;
  left: 0;
}
/*
"podcast--image" />  
                       
"open--preview--button"
                            
*/


/* MODAL */
.modal--overlay {
  position: absolute;
  /* width: 100%; this makes it go over the right edge*/
  height: 100%;
  background-color: rgba(72, 99, 218, 0.6); 
  display: flex;
  justify-content: center;
  align-items: center;
  justify-content: center; /* Center horizontally */
  align-items: center; /* Center vertically */
}

/* Apply the 'display: none;' to hide the modal by default */
.modal--overlay.hidden {
  display: none;
}

.modal--content { /* styling for all content of clicked podcast*/
  text-align: center; 
}

.selected--podcast--image {
  max-width: 300px;
}

.selected--podcast--season--image {
  max-width: 150px;
}


/* sidebar */

.nav--bar {
  display: flex;
  justify-content: space-between;
  font-size: 18px;

}

.favorites--text {
  font-weight: bold;
}

.favorites--amount--text {
  font-size: 20px;
  color: #918E9B;
}

.nav--items {
  /* margin-right: auto; */
  list-style: none;
  display: flex; /* displays items in a row (next to each other)*/
  align-items: center;
  margin-left: 10%;
}

  .settings--icon {
    width: 6%;
    padding: 5px;
    /* height: auto; doesnt work */
  
  }

  .login--icon {
    width: 6%;

  }

  

/* FOOTER */
.footer {
  display: flex; /* Sets the container to use Flexbox */
  justify-content: center; /* Horizontally centers the content */
}



/* STILL TO DO! MAIN.JSX & SIDEBAR.JSX STYLING FROM CHATGPT */
sidebar.css

/* Parent container for both the sidebar and the main content */
/* Assuming you have a container for your main content with class "main-content" */
/* Adjust this width if you want a different width for your sidebar */
.main-container {
  display: flex;
  height: 100%;
}

/* Optional: Add a border to visually separate the sidebar from the main content */
/* Adjust the border color, size, and style as per your preference */
.main-container {
  border-left: 1px solid #ccc;
}






















```