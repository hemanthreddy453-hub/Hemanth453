# Hemanth453
<script src="https://code.jquery.com/jquery-3.6.3.min.js"></script>
<script>
    $(document).ready(function(){
        var pric
        var dsta
        var tv
        var co
       var from=['-select city-','Delhi','Gwalior','Bhopal','Mumbai']
       from.map((item)=>{
        $('#cf').append($('<option>').text(item))
       })
       from.map((item)=>{
        $('#ct').append($('<option>').text(item))
       })
   

        $('#ct').change(function(){
            var ctf=$('#cf option:selected').text()
            var ctt=$('#ct option:selected').text()
            var clas=$('#cls option:selected').text()
            $('#dist').empty()
            $('#tn').empty()
            if((ctf=='Delhi' && ctt=='Gwalior') || (ctf=='Gwalior' && ctt=='Delhi'))
            {
                var dis='323 km'
                // var tpri=220 Sleeper 3rd AC 2nd AC 1st AC
                // tv=tpri
                var train=['-select train-','Gatiman Exprs','Rajdhani Exprs','Sampark Kranti','Kerala Exprs']
                train.map((item)=>{
                $('#tn').append($('<option>').text(item))
                })
                
                    // if(clas=='Sleeper')
                    // {
                    //     var tpri=220 
                    //     tv=tpri 
                    // }

                    // else if(clas=='3rd AC')
                    // {
                    //     var tpri=1125 
                    //     tv=tpri 
                    // }

                    // else if(clas=='2nd AC')
                    // {
                    //     var tpri=1450
                    //     tv=tpri 
                    // }

                    // else if(clas=='1st AC')
                    // {
                    //     var tpri=1825
                    //     tv=tpri 
                    // }
                
       
            }
            else if((ctf=='Delhi' && ctt=='Bhopal') || (ctf=='Bhopal' && ctt=='Delhi'))
            {
                var dis='751 km'
                var tpri=280
                tv=tpri
                var train=['-select train-','CSMT Rajdhani','Bhopal Shatabdi','NZM UBL SF EXPRS','AP Exprs']
                train.map((item)=>{
                $('#tn').append($('<option>').text(item))
       })
                
            }
            else if((ctf=='Delhi' && ctt=='Mumbai') || (ctf=='Mumbai' && ctt=='Delhi'))
            {
                var dis='1365.3 km'
                var tpri=570
                tv=tpri
                var train=['-select train-','MMCT Tejas','BDTS Garibrath','TVC Rajdhani','CSMT Rajdhani']
                train.map((item)=>{
                $('#tn').append($('<option>').text(item))
       })
            }
            else if((ctf=='Gwalior' && ctt=='Bhopal') || (ctf=='Bhopal' && ctt=='Gwalior'))
            {
                var dis='432 km'
                var tpri=250
                tv=tpri
                var train=['-select train-','Bhopal Shtbdi','CSMT Rajdhani','Sampark Kranti','Kerala Exprs']
                train.map((item)=>{
                $('#tn').append($('<option>').text(item))
       })
            } 
            else if((ctf=='Gwalior' && ctt=='Mumbai') || (ctf=='Mumbai' && ctt=='Gwalior'))
            {
                var dis='1090.3 km'
                var tpri=525
                tv=tpri
                var train=['-select train-','Mngla Lksdp','CSMT Rajdhani','Punjab Mail','ASR CSMT Exprs']
                train.map((item)=>{
                $('#tn').append($('<option>').text(item))
       })
            }
            else if((ctf=='Bhopal' && ctt=='Mumbai') || (ctf=='Mumbai' && ctt=='Bhopal'))
            {
                var dis='775.2 km'
                var tpri=385
                tv=tpri
                var train=['-select train-','Lashkar Exprs','CSMT Rajdhani','Mngla Lksdp','Kushinagar Exprs']
                train.map((item)=>{
                $('#tn').append($('<option>').text(item))
       })
            }
            $('#dist').html(dis)
            dsta=dis
            // $('#di').html(dis)
        })




        

        $('#cls').change(function(){
            var ctf=$('#cf option:selected').text()
            var ctt=$('#ct option:selected').text()
            var clas=$('#cls option:selected').text()
            if((ctf=='Delhi' && ctt=='Gwalior') || (ctf=='Gwalior' && ctt=='Delhi'))
            {
                
                    if(clas=='Sleeper')
                    {
                        var tpri=220 
                        tv=tpri 
                        var coach='S1'
                        co=coach
                    }

                    else if(clas=='3rd AC')
                    {
                        var tpri=1125 
                        tv=tpri 
                        var coach='C1' 
                        co=coach
                    }

                    else if(clas=='2nd AC')
                    {
                        var tpri=1450
                        tv=tpri 
                        var coach='B1'
                        co=coach
                    }

                    else if(clas=='1st AC')
                    {
                        var tpri=1825
                        tv=tpri 
                         var coach='A1' 
                        co=coach
                    }
                
       
            }
            else if((ctf=='Delhi' && ctt=='Bhopal') || (ctf=='Bhopal' && ctt=='Delhi'))
            {
                if(clas=='Sleeper')
                    {
                        var tpri=375
                        tv=tpri 
                        var coach='S1'
                        co=coach
                    }

                    else if(clas=='3rd AC')
                    {
                        var tpri=1645 
                        tv=tpri 
                        var coach='C1' 
                        co=coach
                    }

                    else if(clas=='2nd AC')
                    {
                        var tpri=2260
                        tv=tpri 
                        var coach='B1'
                        co=coach
                    }

                    else if(clas=='1st AC')
                    {
                        var tpri=2780
                        tv=tpri 
                         var coach='A1' 
                        co=coach
                    }

            }
            else if((ctf=='Delhi' && ctt=='Mumbai') || (ctf=='Mumbai' && ctt=='Delhi'))
            {
                if(clas=='Sleeper')
                    {
                        var tpri=560 
                        tv=tpri 
                        var coach='S1'
                        co=coach
                    }

                    else if(clas=='3rd AC')
                    {
                        var tpri=1460
                        tv=tpri 
                        var coach='C1' 
                        co=coach
                    }

                    else if(clas=='2nd AC')
                    {
                        var tpri=2085
                        tv=tpri 
                        var coach='B1'
                        co=coach
                    }

                    else if(clas=='1st AC')
                    {
                        var tpri=3535
                        tv=tpri 
                         var coach='A1' 
                        co=coach
                    }
            }
            else if((ctf=='Gwalior' && ctt=='Bhopal') || (ctf=='Bhopal' && ctt=='Gwalior'))
            {
               
                if(clas=='Sleeper')
                    {
                        var tpri=255
                        tv=tpri 
                        var coach='S1'
                        co=coach
                    }

                    else if(clas=='3rd AC')
                    {
                        var tpri=655 
                        tv=tpri 
                        var coach='C1' 
                        co=coach
                    }

                    else if(clas=='2nd AC')
                    {
                        var tpri=910
                        tv=tpri 
                        var coach='B1'
                        co=coach
                    }

                    else if(clas=='1st AC')
                    {
                        var tpri=1510
                        tv=tpri 
                         var coach='A1' 
                        co=coach
                    }
            } 
            else if((ctf=='Gwalior' && ctt=='Mumbai') || (ctf=='Mumbai' && ctt=='Gwalior'))
            {
                if(clas=='Sleeper')
                    {
                        var tpri=525
                        tv=tpri 
                        var coach='S1'
                        co=coach
                    }

                    else if(clas=='3rd AC')
                    {
                        var tpri=2460 
                        tv=tpri 
                        var coach='C1' 
                        co=coach
                    }

                    else if(clas=='2nd AC')
                    {
                        var tpri=3370
                        tv=tpri 
                        var coach='B1'
                        co=coach
                    }

                    else if(clas=='1st AC')
                    {
                        var tpri=4195
                        tv=tpri 
                         var coach='A1' 
                        co=coach
                    }
            }
            else if((ctf=='Bhopal' && ctt=='Mumbai') || (ctf=='Mumbai' && ctt=='Bhopal'))
            {
                if(clas=='Sleeper')
                    {
                        var tpri=420 
                        tv=tpri 
                        var coach='S1'
                        co=coach
                    }

                    else if(clas=='3rd AC')
                    {
                        var tpri=1990
                        tv=tpri 
                        var coach='C1' 
                        co=coach
                    }

                    else if(clas=='2nd AC')
                    {
                        var tpri=2700
                        tv=tpri 
                        var coach='B1'
                        co=coach
                    }

                    else if(clas=='1st AC')
                    {
                        var tpri=3355
                        tv=tpri 
                         var coach='A1' 
                        co=coach
                    }
            }
            $('#dist').html(dis)
            dsta=dis
            // $('#di').html(dis)
        })




        $('#book').click(function(){
            
            var i=tq.value
            $('#ticket').empty() 
            if(tq.value==1)
            {
                var ti=`<table class="tbl3" border=0 width=500px ><tr><img src="trlogo.png" width=500px></tr><tr><th>${$('#cf option:selected').text()} To ${$('#ct option:selected').text()}</th><th width=160px>Train</th></tr><tr><th>Passengers Details</th><th width=160px>${$('#tn option:selected').text()}</th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th>Name</th><th>Age</th><th>Gender</th><th>Birth</th><th width=160px>${cls.value}</th></tr><tr><th>${n1.value}</th><th>${a1.value}</th><th>${g1.value}</th><th>${co},${bt1.value},1</th><th id="di" width=160px>Dist:${dsta}</th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th width=340px>Total Fare</th><th width=161px>Rs ${pric} </th></tr></table>`
            }
            if(tq.value==2)
            {
                var ti=`<table class="tbl3" border=0 width=500px ><tr><img src="trlogo.png" width=500px></tr><tr><th>${$('#cf option:selected').text()} To ${$('#ct option:selected').text()}</th><th width=160px>Train</th></tr><tr><th>Passengers Details</th><th width=160px>${$('#tn option:selected').text()}</th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th>Name</th><th>Age</th><th>Gender</th><th>Birth</th><th width=160px>${cls.value}</th></tr><tr><th>${n1.value}</th><th>${a1.value}</th><th>${g1.value}</th><th>${co},${bt1.value},1</th><th id="di" width=160px>Dist:${dsta}</th></tr><tr><th>${n2.value}</th><th>${a2.value}</th><th>${g2.value}</th><th>${co},${bt2.value},2</th><th id="di" width=160px></th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th width=340px>Total Fare</th><th width=161px>Rs ${pric} </th></tr></table>`
            }

            if(tq.value==3)
            {
                var ti=`<table class="tbl3" border=0 width=500px ><tr><img src="trlogo.png" width=500px></tr><tr><th>${$('#cf option:selected').text()} To ${$('#ct option:selected').text()}</th><th width=160px>Train</th></tr><tr><th>Passengers Details</th><th width=160px>${$('#tn option:selected').text()}</th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th>Name</th><th>Age</th><th>Gender</th><th>Birth</th><th width=160px>${cls.value}</th></tr><tr><th>${n1.value}</th><th>${a1.value}</th><th>${g1.value}</th><th>${co},${bt1.value},1</th><th id="di" width=160px>Dist:${dsta}</th></tr><tr><th>${n2.value}</th><th>${a2.value}</th><th>${g2.value}</th><th>${co},${bt2.value},2</th><th id="di" width=160px></th></tr><tr><th>${n3.value}</th><th>${a3.value}</th><th>${g3.value}</th><th>${co},${bt3.value},3</th><th id="di" width=160px></th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th width=340px>Total Fare</th><th width=161px>Rs ${pric} </th></tr></table>`
            }

            if(tq.value==4)
            {
                var ti=`<table class="tbl3" border=0 width=500px ><tr><img src="trlogo.png" width=500px></tr><tr><th>${$('#cf option:selected').text()} To ${$('#ct option:selected').text()}</th><th width=160px>Train</th></tr><tr><th>Passengers Details</th><th width=160px>${$('#tn option:selected').text()}</th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th>Name</th><th>Age</th><th>Gender</th><th>Birth</th><th width=160px>${cls.value}</th></tr><tr><th>${n1.value}</th><th>${a1.value}</th><th>${g1.value}</th><th>${co},${bt1.value},1</th><th id="di" width=160px>Dist:${dsta}</th></tr><tr><th>${n2.value}</th><th>${a2.value}</th><th>${g2.value}</th><th>${co},${bt2.value},2</th><th id="di" width=160px></th></tr><tr><th>${n3.value}</th><th>${a3.value}</th><th>${g3.value}</th><th>${co},${bt3.value},3</th><th id="di" width=160px></th></tr><tr><th>${n4.value}</th><th>${a4.value}</th><th>${g4.value}</th><th>${co},${bt4.value},4</th><th id="di" width=160px></th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th width=340px>Total Fare</th><th width=161px>Rs ${pric} </th></tr></table>`
            }

            if(tq.value==5)
            {
                var ti=`<table class="tbl3" border=0 width=500px ><tr><img src="trlogo.png" width=500px></tr><tr><th>${$('#cf option:selected').text()} To ${$('#ct option:selected').text()}</th><th width=160px>Train</th></tr><tr><th>Passengers Details</th><th width=160px>${$('#tn option:selected').text()}</th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th>Name</th><th>Age</th><th>Gender</th><th>Birth</th><th width=160px>${cls.value}</th></tr><tr><th>${n1.value}</th><th>${a1.value}</th><th>${g1.value}</th><th>${co},${bt1.value},1</th><th id="di" width=160px>Dist:${dsta}</th></tr><tr><th>${n2.value}</th><th>${a2.value}</th><th>${g2.value}</th><th>${co},${bt2.value},2</th><th id="di" width=160px></th></tr><tr><th>${n3.value}</th><th>${a3.value}</th><th>${g3.value}</th><th>${co},${bt3.value},3</th><th id="di" width=160px></th></tr><tr><th>${n4.value}</th><th>${a4.value}</th><th>${g4.value}</th><th>${co},${bt4.value},4</th><th id="di" width=160px></th></tr><tr><th>${n5.value}</th><th>${a5.value}</th><th>${g5.value}</th><th>${co},${bt5.value},5</th><th id="di" width=160px></th></tr></table><table class="tbl3"  border="1" width="500px"><tr><th width=340px>Total Fare</th><th width=161px>Rs ${pric} </th></tr></table>`
            }
            $('#ticket').html(ti)
        })
     
        $('#tq').keyup(function(){
            var i=tq.value
            $('#result').empty()
           if(tq.value==1){
            var msg=`<table border="1" class="tbl2"><caption>Passenger Details:</caption><tr><th>S.No.</th><th>Name</th><th>Age</th>
        <th>Gender</th><th>Birth Type</th></tr><tr><th>1.</th><td><input type="text" id="n1" class="fld2"></td><td><input type="text" id="a1" class="fld2"></td><td><select  id="g1" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt1" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr></table>`
           }

          else if(tq.value==2){
            var msg=`<table border="1" class="tbl2"><caption>Passenger Details:</caption><tr><th>S.No.</th><th>Name</th><th>Age</th>
        <th>Gender</th><th>Birth Type</th></tr><tr><th>1.</th><td><input type="text" id="n1" class="fld2"></td><td><input type="text" id="a1" class="fld2"></td><td><select  id="g1" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt1" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>2.</th><td><input type="text" id="n2" class="fld2"></td><td><input type="text" id="a2" class="fld2"></td><td><select  id="g2" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt2" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr></table>`
           }

           else if(tq.value==3){
            var msg=`<table border="1" class="tbl2"><caption>Passenger Details:</caption><tr><th>S.No.</th><th>Name</th><th>Age</th>
        <th>Gender</th><th>Birth Type</th></tr><tr><th>1.</th><td><input type="text" id="n1" class="fld2"></td><td><input type="text" id="a1" class="fld2"></td><td><select  id="g1" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt1" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>2.</th><td><input type="text" id="n2" class="fld2"></td><td><input type="text" id="a2" class="fld2"></td><td><select  id="g2" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt2" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>3.</th><td><input type="text" id="n3" class="fld2"></td><td><input type="text" id="a3" class="fld2"></td><td><select  id="g3" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt3" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr></table>`
           }

           else if(tq.value==4){
            var msg=`<table border="1" class="tbl2"><caption>Passenger Details:</caption><tr><th>S.No.</th><th>Name</th><th>Age</th>
        <th>Gender</th><th>Birth Type</th></tr><tr><th>1.</th><td><input type="text" id="n1" class="fld2"></td><td><input type="text" id="a1" class="fld2"></td><td><select  id="g1" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt1" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>2.</th><td><input type="text" id="n2" class="fld2"></td><td><input type="text" id="a2" class="fld2"></td><td><select  id="g2" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt2" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>3.</th><td><input type="text" id="n3" class="fld2"></td><td><input type="text" id="a3" class="fld2"></td><td><select  id="g3" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt3" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>4.</th><td><input type="text" id="n4" class="fld2"></td><td><input type="text" id="a4" class="fld2"></td><td><select  id="g4" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt4" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr></table>`
           }

           else if(tq.value==5){
            var msg=`<table border="1" class="tbl2"><caption>Passenger Details:</caption><tr><th>S.No.</th><th>Name</th><th>Age</th>
        <th>Gender</th><th>Birth Type</th></tr><tr><th>1.</th><td><input type="text" id="n1" class="fld2"></td><td><input type="text" id="a1" class="fld2"></td><td><select  id="g1" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt1" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>2.</th><td><input type="text" id="n2" class="fld2"></td><td><input type="text" id="a2" class="fld2"></td><td><select  id="g2" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt2" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>3.</th><td><input type="text" id="n3" class="fld2"></td><td><input type="text" id="a3" class="fld2"></td><td><select  id="g3" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt3" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>4.</th><td><input type="text" id="n4" class="fld2"></td><td><input type="text" id="a4" class="fld2"></td><td><select  id="g4" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt4" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr><tr><th>5.</th><td><input type="text" id="n5" class="fld2"></td><td><input type="text" id="a5" class="fld2"></td><td><select  id="g5" class="fld2"><option>-select-</option><option>Male</option><option>Female</option><option>Others</option></select></td><td><select  id="bt5" class="fld2"><option>-select-</option><option>Upper</option><option>Middle</option><option>Lower</option><option>Side Upper</option><option>Side Lower</option></select></td></tr></table>`
           }
            $('#result').html(msg)
            var pri=i*tv
            pric=pri
            $('#price').html(pri)
        })
    })

</script>
<html>
    <style>
.bdy{
    background-image: url("trn.gif");
    background-size: cover;
}

.tbl1{
     background-color: rgb(91, 26, 26);
     color: white;
     border-radius: 25px;
}
.fld1{
    background-color: black;
    color: aqua;
    border-radius: 25px;
}
.tbl2{
    background-color: black;
    color: white;
}
.fld2{
    background-color: black;
    color: aqua;
    border-radius: 25px;
}
.btn{
    background-color: aqua;
    color: black;
    border-radius: 25px;
    font-weight: bolder;
}
.btn:hover{
    background-color: white;
    color: black;
}
.tbl3{
    background-color: rgb(255, 184, 136);
}
    </style>
    <body class="bdy">
     <center>
      <h2  class="tbl2">"Welcome To The Railway Reservation System"<br>-----------------------------------------------------------</h2><br>
        <table border="0" class="tbl1" width="400px"><tr><th> City From:</th><th><select  id="cf" class="fld1"></select></th></tr><tr><th>City To:</th><th><select  id="ct" class="fld1"></select></th></tr><tr><th>Train Name:</th><th><select  id="tn" class="fld1"><option>-select train-</option></select></th></tr><tr><th>Class:</th><th><select  id="cls" class="fld1"><option>-select-</option><option>Sleeper</option><option>3rd AC</option><option>2nd AC</option><option>1st AC</option></select></th></tr>
        <tr><th>Tickets:</th><th><input type="text" id="tq" placeholder="max 5 Tickets can be booked " class="fld1"></th></tr><tr><th>Distance:</th><th><span id="dist"></span></th></tr><tr><th>Price:</th><th><span id="price"></span></th></tr></table><br><br>
        <div id="result"></div><br><br>
        <input type="button" value="Book Ticket" id="book" class="btn"><br><br><br><br>
        <div id="ticket"></div>

        
    </center>
</body>
</html>
