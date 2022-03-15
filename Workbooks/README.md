# Workbooks


<details> 
  <summary>TIL:</summary>
  <details>
    <summary>2022-03-14</summary>
    For some reason workbook template cannot be used. Need to investigate why.
    In ARM-template there's "workbookId": { ... defaultValue: "[newGuid()]" and this generates new guid.
    This new guid creates a confict for existing dashboard and github workflow will result as failed.
    Generated a static guid for defaultValue and now workflow works. 
  </details><!--2022-03-14-->
 </details<!--TIL-->
