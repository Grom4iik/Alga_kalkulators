# Alga_kalkulators
WEB uzdevums

<script type="text/javascript">
function compute() {
	with (document.paycheck) {
		otrate.value = rate.value * otpercent.value;
		gross.value = (rate.value * hours.value) + otrate.value * ot.value;
		tax.value = gross.value * taxrate.value;
		total.value = gross.value - tax.value - other.value;
   }
}
</script>
<html>
<HEAD>
    <meta http-equiv="Content-Type" content="text/html"; charset="utf-8">
    <title>Algu kalkulators</title>

</HEAD>
<BODY vlink="#0000ff"; style="background-image: url('https://img.freepik.com/premium-photo/halloween-wallpapers-for-the-desktop_900101-27453.jpg');
                              background-size: cover;
							  background-position: center;}">
    <BR>
	<BR>
	<BR>
    <center>
        <BR><BR>
 
        <BR><BR>
        <table border=0 WIDTH=486 CELLPADDING=3 CELLPADDING=0 bgcolor="#c0c0c0">
            <tr><td>
			<FONT size="+2" face="Helvetica,Arial">	
			<FONT color="#006666"><b>Algu kalkulators</b></font></font>
                <BR><BR>
                Ievadot algas likmi un nostrādāto stundu skaitu un pēc izvēles jebkuras virsstundas un algas likmi, savu nodokļu likmi un citus secinājumus. Uzziniet, no kurienes nāk jūsu nauda un kur tā nonāk.
				<BR>
                <HR>
            </td></tr>
        </table>


    <center>
    <form name=paycheck>
		<table border=1 bgcolor="#c0c0c0">
			<tr>
				<td bgcolor="#c0c0c0" align=right><b>Maksājuma likme:</b></td>
				<td><input type=text name=rate size=5></td>
				<td bgcolor="#c0c0c0" align=right>Stundas:</b></td>
				<td><input type=text name=hours size=5></td>
			</tr>
			<tr>
				<td align=right>Virsstundu likme:</td>
				<td><input type=text name=otpercent size=5 value=1.5></td>
				<td align=right>Virsstundas:</td>
				<td><input type=text name=ot size=5 value=0></td>
			</tr>
			<tr>
				<td align=right>Stundu likme par virsstundām:</td>
				<td><input type=text name=otrate size=5></td>
				<td align=right>Kopējā alga:</td> 
				<td><input type=text name=gross size=5></td>
			</tr>
			<tr>
				<td colspan=2>&nbsp; &nbsp;</td>
				<td align=right><p>Nodokļa likme:</td>
				<td><input type=text name=taxrate value=.12 size=5></td>
			</tr>
			<tr>
				<td colspan=2>&nbsp; &nbsp;</td>
				<td align=right>Vispārējie nodokļi:</td>
				<td><input type=text name=tax size=5></td>
			</tr>
			<tr>
				<td colspan=2>&nbsp; &nbsp;</td>
				<td align=right><p>Citi atskaitījumi:</td>
				<td><input type=text name=other value=0 size=5></td>
			</tr>
			<tr>
				<td colspan=2>&nbsp; &nbsp;</td>
				<td align=right bgcolor="#ffff80"><b>Jūsu ienākumi:</b></td>
				<td><input type=text name=total size=5></td>
			</tr>
			<tr>
				<td colspan=4 align=center><input type=button value="Aprēķināt" onClick="compute()"></td>
			</tr>
		</table>
	</form>
	</center>
	
</BODY>
</html>
