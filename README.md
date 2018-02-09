# unique
利用对象思想做数组去重


//数组去重: 
   let ary=[1,2,3,4,2,3]
   function uique(ary){
      let obj={};
      for(var i=0;i<ary.length;i++){
            if(obj[ary[i]]==ary[i]){
                ary.splice(i,1);
                i--;
                continue;
            } 
            obj[ary[i]]=ary[i];
       }
       obj=null;
       
    }
  
    uique(ary);
