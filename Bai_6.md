# Bai_6
<!DOCTYPE html>
<html>
<head>
	<title> Bài 6</title>
</head>
<script language="javascript">
function checkAll(){
	var txtStock = fm.txtStock.value;
	if(txtStock == ""){
		alert("Khong duoc de trong du lieu");
		fm.txtStock.focus();
		return false;
		}
		//kiem tra gia tri truong radiobutton
	var cnt = 0;
	var t1;
	for(var i = 0; i < fm.rad.length; i++){
		if(fm.rad[i].checked == true){
			cnt++;
		}
	}
	if(cnt == 0){
		alert("Phai click vao mot trong 3 truong: beginner/intermeiate/expert");
		return false;
	}
	else{
		for(var j = 0; j <=cnt; j++){
			if(fm.rad[j].checked == true)
				alert(fm.rad[j].value);
		}
		return true;
	}
	
	//Kiem tra gia tri cua truong checkbox
	var cntCheckBox = 0;
	for(var i = 0; i < fm.cb.length; i++){
		if(fm.cb[i].checked == true){
			cntCheckBox++;
		}
	}
	if(cntCheckBox == 0){
		alert("Phai click vao mot trong 3 truong: Individual/Options/Mutual");
		return false;
	}
	
	
	//var strText = "Experience: " + ;
	
	
	return true;
}
</script>
	
	
<body>
<H1 align="left"><FONT SIZE = "6" > Create a Profile</FONT></H1><hr>
<form name="fm" method="post" action="" onSubmit="return checkAll();">

<h3>First Name: 
		<input name="txtStock" type="text" id="txtStock">
	</h3>
<h3>Last Name: 
		<input name="txtStock" type="text" id="txtStock">
	</h3>
	<h3> Date of Birht:
	<select name="select">
			<option value="0"> Month</option>
			<option value="1"> 1</option>
			<option value="2"> 2</option>
			<option value="3"> 3</option>
			<option value="4"> 4</option>
			<option value="5"> 5</option>
			<option value="6"> 6</option>
			<option value="7"> 7</option>
			<option value="8"> 8</option>
			<option value="9"> 9</option>
			<option value="10"> 10</option>
			<option value="11"> 11</option>
			<option value="12"> 12</option>
		</select>
		<select name="select">
		    <option value="0"> Day</option>
			<option value="1"> 1</option>
			<option value="2"> 2</option>
			<option value="3"> 3</option>
			<option value="4"> 4</option>
			<option value="5"> 5</option>
			<option value="6"> 6</option>
			<option value="7"> 7</option>
			<option value="8"> 8</option>
			<option value="9"> 9</option>
			<option value="10"> 10</option>
			<option value="11"> 11</option>
			<option value="12"> 12</option>
			<option value="13"> 13</option>
			<option value="14"> 14</option>
			<option value="15"> 15</option>
			<option value="16"> 16</option>
			<option value="17"> 17</option>
			<option value="18"> 18</option>
			<option value="19"> 19</option>
			<option value="20"> 2</option>
			<option value="21"> 21</option>
			<option value="22"> 22</option>
			<option value="23"> 23</option>
			<option value="24"> 24</option>
			<option value="25"> 25</option>
			<option value="26"> 26</option>
			<option value="27"> 27</option>
			<option value="28"> 28</option>
			<option value="29"> 29</option>
			<option value="30"> 30</option>
			<option value="31"> 31</option>
			</select>
		<select name="select">
			<option value="0"> Year</option>
			<option value="1"> 1980</option>
			<option value="2"> 1981</option>
			<option value="3"> 1982</option>
			<option value="4"> 1983</option>
			<option value="5"> 1984</option>
			<option value="6"> 1985</option>
			<option value="7"> 1986</option>
			<option value="8"> 1987</option>
			<option value="9"> 1988</option>
			<option value="10"> 1989</option>
			<option value="11"> 1990</option>
			<option value="12"> 1991</option>
			<option value="13"> 1992</option>
			<option value="14"> 1993</option>
			<option value="15"> 1994</option>
			<option value="16"> 1995</option>
			<option value="17"> 1996</option>
			<option value="18"> 1997</option>
			<option value="19"> 1998</option>
			<option value="20"> 1999</option>
			<option value="21"> 2000</option>
		</select>
		</h3>
		<h3> Gender:
		<input name="rad" type="radio" value="1"> male
		<input name="rad" type="radio" value="2"> female 
	</h3>
	<p>
	
		<input type="Submit" name="Submit" value="Save">
		</p>
		</form>
</body>
</html>
