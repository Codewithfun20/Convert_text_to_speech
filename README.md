# Convert_text_to_speech
This is text to speech converter
<html>
<style>
#a{
width:600px;
height:100px;
background-color:F4BB44;
}
</style>
<body bgcolor="9FE2BF">
<center>
<br>
<br>
<br>
<br>
<br>
<br>
<div id ="a"><font style="font-size:45px; color:770737;font-famliy:avalon;position:relative; top:26px;"><b>Convert Text To Speech</b></div>
<br>
<textarea placeholder=" Enter text" style="height:400px;width:600px; font-size:25px;" id ="text"></textarea>
<br>
<br>
<button style="height:50px; width:600px;background-color:FBCEB1; font-size:35px;"><b>Speak</b></button>
<br>
<br>
<input type="button" value="Source Code" style="height:50px;width:200px;border-radius:10px;background-color:green;color:white;font-size:30px;" onclick="get()">
</center>
</body>

<script>
utterance=new SpeechSynthesisUtterance()
document.querySelector("button").addEventListener("click", () => {
utterance.text=document.querySelector("textarea").value;
window.speechSynthesis.speak(utterance)
})
function get(){
window.open("https://github.com/Codewithfun20/Convert_text_to_speech/edit/main/README.md")
}
</script>
</html>
