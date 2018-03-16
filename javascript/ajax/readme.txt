var obj = { index: 'contenu' }, string;
string = JSON.stringify(obj);
alert(typeof string + ' : ' + string); // Affiche : « string : {"index":"contenu"} »
obj = JSON.parse(string);
alert(typeof obj + ' : ' + obj); // Affiche : « object : [object Object] »







//XMLHttpRequest
var xhr = new XMLHttpRequest();
xhr.open('GET', 'http://localhost:8080/platform/matching/listreference',true);
xhr.setRequestHeader('Content-Type', 'text/html; charset=UTF-8');
	xhr.send(null);
	var overlay = document.getElementById('overlay');
	var overlay;
	xhr.addEventListener('readystatechange', function() {
		if (xhr.readyState === XMLHttpRequest.DONE && xhr.status === 200) {
// 			alert('statut 200');
			 overlay = document.getElementById('overlay');
			 overlay.innerHTML = xhr.responseText;
		} else if (xhr.readyState === XMLHttpRequest.DONE) {
// 			alert('status here ' + xhr.status);
		} else {
// 			alert('xhr ready state ' + xhr.readyState);
// 			alert('xhr status ' + xhr.status);
		}
	});
	

	
	
	
	
	
	
	
	
	
	
	
encodage a voir




















autoriser les cross domain request 
XHR2  firefox6 , chrome13 
sur xhr1 on fait abort couplé avec setTimeout(function,70000)
xhr.timeout = 10000; // La requête se terminera si elle n'a pas abouti au bout de 10 secondes







envoies des cookies 
xhr.withCredentials = true;