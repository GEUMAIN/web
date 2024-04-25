### 등록 사이트 CSS로 꾸미기

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Insert title here</title>
<style>
    table, th, td { 
    	border: 2px solid black;
    	}
    table {border-collapse : collapse}
    .Vtable {
    	position: absolute;
  		top: 45%;
  		left: 25%;
  		margin: -25px 0 0 -25px;
    }
    .Vtitle {
    	position: absolute;
  		top: 25%;
  		left: 33%;
  		margin: -25px 0 50 -25px;
  		border-radius: 25px;
    }
    
    body {
    	height: 100vh;
    	background: linear-gradient(#895cf3 50%, #15191f 50%);
    }
    
    
    * {
    	font-family: "Poppins", sans-serif;
    }
    
    .Vtitle {
    	padding : 0 100px 0;
    	background-color : white;
    	color : #895cf3;
    }
</style>
	
</head>
<body>
	<div class="Vtitle">
		<h1>reservation</h1>
	</div>
	<form name="rData" action="" method="post">
	<table width = 60% class = "Vtable" style="background-color:white">
		<tr>
			<th>예약번호</th>
			<td><input type="text" placeholder="예)20210011"></input></td>
			
		</tr>
		<tr>
			<th>주민번호</th>
			<td><input type="text" maxlength="14" placeholder="예)790101-1111111"></input></td>
		</tr>
		<tr>
			<th>백신코드</th>
			<td>
				<select name="V">
					<option value="1" selected> 백신선택
					<option value="2"> A백신
					<option value="3"> B백신
					<option value="4"> C백신
				</select> 예)V001, V002, V003
			</td>
		</tr>
		<tr>
			<th>병원코드</th>
			<td><input type = "radio" name="hos">가_병원</input><input type = "radio" name="hos">나_병원</input><input type = "radio" name="hos">다_병원</input><input type = "radio" name="hos">라_병원</input> 예)H002, H003, H004</td>
		
		</tr>
		<tr>
			<th>병원코드</th>
			<td><input type = "checkbox" name="hos2">가_병원</input><input type = "checkbox" name="hos2">나_병원</input><input type = "checkbox" name="hos3">다_병원</input><input type = "checkbox" name="hos4">라_병원</input> 예)H002, H003, H004</td>
		</tr>
		
		<tr>
			<th>예약날짜</th>
			<td><input type="text" placeholder="예)20210101"></input></td>
		</tr>
		
		<tr>
			<th>예약시간</th>
			<td><input type="text" maxlength="4" placeholder="예)0930, 1130"></input></td>
		</tr>
		
		<tr>
				<td colspan = "2" style = "text-align: center"><input type="submit" value="등록" class="button"><input type="reset" value="취소" class="button"></input></td>
		</tr>
	</table>
	</form>
</body>
</html>
```

### 결과

![image](https://github.com/GEUMAIN/web/assets/128437656/4c70e14d-e990-4a98-9ba3-0703ae7815ef)

