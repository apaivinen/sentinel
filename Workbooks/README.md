# Workbooks


<details> 
  <summary>TIL:</summary>
  <details>
    <summary>2022-03-15</summary>
    Actions resulted to failure everytime even thought workbook was uploaded to sentinel.
    Reason: I had arm template and workbook template. Arm template was uploaded to sentinel but workbook template resulted to an error.
    Removed workbook template.
    At this moment not going to investigate further why workbook tmeplate didn't work as planned.
  </details>
  <details>
    <summary>2022-03-14</summary>
    For some reason workbook template cannot be used. Need to investigate why.
    In ARM-template there's "workbookId": { ... defaultValue: "[newGuid()]" and this generates new guid.
    This new guid creates a confict for existing dashboard and github workflow will result as failed.
    Generated a static guid for defaultValue and now workflow works. 
  </details><!--2022-03-14-->
 </details<!--TIL-->
