# getDate
function getDate(str){
	var word = /^\d\d?-\d\d?-\d{4}$/.test(str);
	if(word === true){
		var result = new Date(str);
		echo(result);
	}else{
		echo(false);
	}
}
getDate("01-20-2014");
