# preloader
This is simple preloader for your website. Just copy the code and pasted into your files.

step 1:
copy HTML stacture from the index file

    <div class="preloader-div">
        <div class="spinner"></div>
    </div>
    
   Paste this code into your index file after the (<body>) body tag.
   
   Step 2:
   
   Paste the CSS into your style css file.
   
   .preloader-div {
    position: absolute;
    width: 100%;
    height: 100%;
    z-index: 999;
    background-color: #ddd;
    left: 0;
    top: 0;
}
.spinner {
    width: 50px;
    height: 50px;
    border: 3px solid #ddd;
    border-top-color: #FF9800;
    border-bottom-color: green;
    border-radius: 100%;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    -webkit-animation: round 1s linear infinite;
            animation: round 1s linear infinite;
}
@-webkit-keyframes round{
	from{-webkit-transform: rotate(0deg);transform: rotate(0deg)}
    to{-webkit-transform: rotate(360deg);transform: rotate(360deg)}
}
@keyframes round{
	from{-webkit-transform: rotate(0deg);transform: rotate(0deg)}
    to{-webkit-transform: rotate(360deg);transform: rotate(360deg)}
}

Step 3:

then active this preloader into your custom js file.

    jQuery(window).load(function(){
        $(".century-preloader").fadeOut(500);
    });
    
    That's it. very sample. you may change your background color, border color .

