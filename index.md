---
layout: default
---

# ConfigMgr It's not Dead

![image](https://github.com/JordanTheITGuy/IsConfigMGrDead/blob/master/assets/images/IsConfigMgrDead.png?raw=true/)

[![alt text](https://raw.githubusercontent.com/JordanTheITGuy/IsConfigMGrDead/master/assets/images/MicrosoftLogopng.png)](https://www.youtube.com/embed/DnmnLr2NUXk?start=1105 "Brad Anderson - On ConfigMgr")



This whole website started as the child of a joke on Twitter. A joke that just kept going on and on until this website was born. 

## images1
<script>
var bCheckEnabled = true;
var bFinishCheck = false;

var img;
var imgArray = new Array();
var i = 0;

var myInterval = setInterval(loadImage, 1);

function loadImage() {

    if (bFinishCheck) {
        clearInterval(myInterval);
        alert('Loaded ' + i + ' image(s)!)');
        return;
    }

    if (bCheckEnabled) {

        bCheckEnabled = false;

        img = new Image();
        img.onload = fExists;
        img.onerror = fDoesntExist;
        img.src = 'images/' + i + '.png';
        document.body.appendChild(img);
    }

}

function fExists() {
    imgArray.push(img);
    i++;
    bCheckEnabled = true;
}

function fDoesntExist() {
    bFinishCheck = true;
}
</script>

<iframe width="560" height="315" src="https://www.youtube.com/embed/DnmnLr2NUXk?start=1105" frameborder="0" allowfullscreen></iframe>

