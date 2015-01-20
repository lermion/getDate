# getDate

function getDate(str){
	var f = str.match(/^(\d\d?)-(\d\d?)-(\d{4})$/);
	if(f){
		return new Date(f[3], f[2] -1, f[1]);
	}
}
var d = getDate("21-10-2014");
echo(d.toString());
