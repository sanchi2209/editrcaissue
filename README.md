<!-- this is for the popup modal page -->
<div class="modal fade show" id="popupContainer"  role="dialog" aria-modal="true" style="display: none; padding-right: 17px;">
  <div class="modal-dialog modal-xl modal-dialog-scrollable" role="document">
      <div class="modal-content">
          <div class="modal-header">
            <header class="sysbar">
              <div class="items-container">
                <div class="item" routerLink="/">
                  <!-- <i class="icon icon-econ"></i> -->
                  <span class="product"></span>
                  <span class="acronym"></span>
                </div>
               </div>
               <div class="middiv">
                <div class="item">
          
                  <span class="product" style="font-size: 14px;font-family: Ericsson Hilda;text-align: center;">Event Manager</span>
                  
                  <!-- <i class="icon icon-econ" style="margin-left: 5px;"></i> -->
          
                </div>
              </div>
             
            </header>
           
          </div>
           
           
          <div id="modal_dialog_body" class="modal-body" style="position: relative;-webkit-box-flex: 1; -ms-flex: 1 1 auto;flex: 1 1 auto;padding: 25px 30px;">
            <div class="row">
              <div class="col">
                <div  id="section1" style="width:100%">
                       <h4>Event
                         Information:</h4>
                         <hr>
                     <div id="popupContent" style="text-align: left;font-size: 13px;margin-bottom:10px;font-family:Ericsson Hilda;margin-left:20px;margin-top:15px;">
                     </div>
                    <div class="section3">
                      <h4> Additional Info: </h4>
                       <hr>
                     <div style="display: table;  width: 100%;margin-top:10px;" id="tablecol">
                       <div style="display: table-row;display: flex;
                       flex-direction: row; align-items: flex-start;">
                         <div style="display: table-cell; white-space: nowrap; padding-right: 95px; padding-left:20px;font-size:13px;"><strong>RCA</strong></div>
                         <div style="display: table-cell; text-align: center; width: 10px; padding: 0 16px;">:</div>
                         <div  style="display: table-cell; white-space: nowrap; padding-left: 10px;" >
                         <!-- <form name="rcaform"  id="rcaform" onsubmit="submitrcasummaryform(event)" method="POST"> -->
                           <p style="margin-bottom:0px;display: flex;flex-direction: row;align-items: center;height:100%;width:100%;">
                        
                             <input type="text" id="rcatext"  name="rca"   placeholder="Enter rca"  style="width:100%;height:100%;border:1px solid black;"/>
                            
                          
                          
                             <button class="btn" id="rcaeditbtn" style="margin-left:0px;padding:0px;min-width:40px;font-size:12px;" onclick="EditRcaSummaryForm((document.getElementById('rsde3key').placeholder))">Edit</button>
                           <button class = "btn" id="rcasubmitbtn"  style="margin-left:5px;padding:0px;min-width:40px;font-size:12px;" onclick="submitrcasummaryform((document.getElementById('rsde3key').placeholder))">Submit</button>
                          </p>
                         </div>  
                         </div>
                         <div  style="display: table-row; display: flex;
                         flex-direction: row;
                         align-items: flex-start; margin-bottom: 10px;">
                           <div style="display: table-cell; white-space: nowrap; padding-right: 30px; padding-left:20px;padding-bottom:10px;font-size:13px;"><strong>Recovery Team</strong></div>
                           <div style="display: table-cell; text-align: center; width: 10px; padding: 0 16px;">:</div>
                           <div   style="display: table-cell; white-space: nowrap; padding-left: 10px;" >
                             <textarea id="CIDInput" type="text" oninput="auto_growCid(this)"   placeholder="enter cid Information" style="min-width: 170%;
                             min-height: 10vh;
                             margin-top: 8px;
                             overflow: hidden;
                             font-size: 12px;
                             font-family: Ericsson Hilda;
                             height: 308px;" ></textarea>
                           <!-- <button onclick="addCIDComment()" style="margin-top: 5px; background-color: #0064bd; color:white;border-color: transparent; border-radius: 2px;">Submit</button> -->
                           <!-- <button  class="btn" id="editcidsummary" onclick="EditcidSummaryForm()" style="margin-left:0px;padding:0px;min-width:40px;font-size:12px;">Edit</button> -->
         <div>   
                           <button class="btn" id="cideditbtn" style="padding:0px;margin-left:0px;min-width:40px;font-size:12px;" onclick="EditcidSummaryForm(document.getElementById('rsde3key').placeholder)" >Edit</button>
                           <button class="btn" id="cidsubmitbtn" onclick="submitcidsummaryform(document.getElementById('rsde3key').placeholder)" style="margin-left:0px;padding:0px;min-width:40px;font-size:12px;">Submit</button>
         </div>
                           </div>
                           </div> 
                       </div>
                   <!-- </div> -->
                    
                   </div>
                </div>
                   
              </div>
      <div class="col">
        <div id="section2">
    <h4>Incident Executive  Summary</h4>
            <hr>
       <div class="content">
         
         <div class="executivesummarycontainer" style="width:100%">
           <p style="margin-bottom:0px;display: flex;flex-direction: row;align-items: center;width:100%;">
              
            <textarea  type="text" id="executivetext" oninput="auto_grow(this)"
             placeholder="Enter Incident status summary here"   name="summary" style="min-width: 100vh;min-height:10vh;display: flex;border: none;overflow: hidden;font-size: 12px;font-family:Ericsson Hilda;" disabled="disabled"></textarea>
</p>  
<div style="display:flex; justify-content:flex-end;margin-right:12%;"> 
               <button class="btn" id="summaryeditbtn"  style="margin-left:0px;padding:0px;min-width:40px;font-size:12px;" onclick="EditSummaryForm((document.getElementById('rsde3key').placeholder))">Edit</button>
             <button class="btn" id="summarysubmitbtn"  style="margin-left:5px;padding:0px;min-width:40px;font-size:12px;" onclick="submitsummaryform((document.getElementById('rsde3key').placeholder))">Submit</button>
</div>
             <!-- </form> -->
          </div>
   
      
       </div>
     
         </div>
        
      </div>
</div>
</div>
          <div class="modal-footer pt-3 m-0">
              <button type="button" class="btn btn-danger" data-dismiss="modal" onclick="closePopup1()" id="close">Close</button>
          </div>
      </div>
  </div>
</div>



<script>
  async function openPopupClosedtickets(key) {
  debugger
  globlKey=key;
 
  const url = `http://localhost:5502/frontend/FrontOffice.html?&incidentkey=${globlKey}`;
window.open(url, '_blank');

  //
  console.log("getting 1st popup key",globlKey);
  // event.preventDefault();
  const text= document.getElementById('rsde3key');
  text.placeholder=globlKey;
  console.log("rsde3key",document.getElementById("rsde3key").placeholder)
  
  try{
   
    fetch('http://localhost:3000/backend/jira-data', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',

      },
        body: JSON.stringify({

          "jql":"project = DE3 AND labels in (Critical,critical) and resolution = Resolved  and resolutiondate >= -60D ORDER BY created DESC",
          "startAt": 0,

          "maxResults": 1000,

      }),
    
    })
      .then((res) => {
        return res.json()
        
      }).then((data) => {
        //  document.body.innerHTML += ('Response data', data)
       
        // populateFormFields();
        
       
        const popupContent = document.getElementById("popupContent");
        let popupContentHTML = "";
            data.issues.forEach((issue) => {
              if (issue.key == key) {
                
              
               
                // console.log("Ticket ID;,ticketKey");
                
                    updateTimeline1(key);
                   
                rcadata(key);
                rcasummary(key);
                 document.getElementById('cideditbtn').addEventListener("click", EditcidSummaryForm(globlKey));
                   document.getElementById('rcaeditbtn').addEventListener("click",EditRcaSummaryForm(globlKey)) ;
                   document.getElementById('summarysubmitbtn').addEventListener("click", EditSummaryForm(globlKey))
                
                   fetchcomments(globlKey)
                const createddata=issue.fields.created.replace(/(\.\d{3}[+-]\d{4})$/, '')
              //  const remainingTime = issue.fields.customfield_13913.ongoingCycle.remainingTime?.friendly;; 
              //  console.log(remainingTime)
              // const formattedTime = remainingTime.replace(/(-?\d+)h (\d+)m/, (_, h, m) => `${Math.floor(h / 24)}d ${h % 24}h ${m}m`);
//               <div style="display: table-row; margin-bottom: 10px;">
                
             
               fetch(`http://localhost:3000/backend/rca/rcagetdata/${globlKey}`)
               .then((res)=> res.json())
               .then((data=>{
                if(data.length>0){
                  rcaValue=data[data.length-1].RCA;
                  console.log("data length",data.length-1)
              document.getElementById("rsde3key").value=data[data.length-1].ticketkey;

                  console.log("rcavalu ",typeof(rcaValue));
                }
                 
                  console.log("gettung rca value",rcaValue)
               }))
              // .then(()=>{
               
              // }
              // )
               
          

             
// const RcaData= localStorage.getItem("rcainformation");
// console.log(RcaData);
popupContentHTML += `

<div style="display: table; width: 100%;">

<div style="display: table-row; margin-bottom: 10px;">

<div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Incident</strong></div>

<div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

<div style="display: table-cell; white-space: nowrap; padding-left: 20px;">  <a href="https://eteamproject.internal.ericsson.com/servicedesk/customer/portal/1/${issue.key}" target="_blank" >${issue.key}</a></div>

</div>

<div style="display: table-row; margin-bottom: 10px;">

        <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Slogan</strong></div>

        <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

        <div style="display: table-cell; white-space: pre-wrap; padding-left: 20px;">${issue.fields.summary}</div>

    </div>

    <div style="display: table-row; margin-bottom: 10px;">

        <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Incident Priority</strong></div>

        <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

        <div style="display: table-cell; white-space: nowrap; padding-left: 20px;">${issue.fields.priority.name}</div>

    </div>
    <div style="display: table-row; margin-bottom: 10px;">

        <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Reporter</strong></div>

        <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

        <div style="display: table-cell; white-space: nowrap; padding-left: 20px;">${issue.fields.reporter.displayName}</div>

    </div>
    <div style="display: table-row; margin-bottom: 10px;">

    <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Assignee</strong></div>

    <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

    <div style="display: table-cell; white-space: nowrap; padding-left: 20px;">${issue.fields.assignee.displayName}</div>

</div>
<div style="display: table-row; margin-bottom: 10px;">

    <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Incident Reported</strong></div>

    <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

    <div style="display: table-cell; white-space: nowrap; padding-left: 20px;">${createddata}</div>

</div>
<div style="display: table-row; margin-bottom: 10px;">

    <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>Labels</strong></div>

    <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

    <div style="display: table-cell; white-space: nowrap; padding-left: 20px;">${issue.fields.labels}</div>

</div>


<div style="display: table-row; margin-bottom: 10px;">

    <div style="display: table-cell; white-space: nowrap; padding-right: 20px; padding-bottom:10px;"><strong>User Origination</strong></div>

    <div style="display: table-cell; text-align: center; width: 10px; padding: 0 10px;">:</div>

    <div style="display: table-cell; white-space: nowrap; padding-left: 20px;">${issue.fields.customfield_12650.value}</div>

</div>

                          
                     
</div>

`;                
// popupContentHTML += `


`
              
                                 `
                     } 
       

            });
            popupContentHTML +=``
            popupContent.innerHTML = popupContentHTML;
            popupContainer.style.display = "block";
        
      })
      
  }catch(error){
    console.error("error fetching data", error);
  }
  

    
   
  }
</script>
