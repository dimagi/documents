
# Get Requisition Details API Specifications

### Communication Type

- GET, to OpenLMIS

### Parameters

- username - Mandatory (Post Request Header)
- password - Mandatory (Post Request Header)
- requisitionId - Mandatory

### Return

- Complete Requisition JSON

### Dependencies

- username
- password
- requisitionId

### Notes

- CommTrack will retain the RequisitionID generated for each Report submitted to OpenLMIS.

### JSON Example

{"rnr":{"id":1,"modifiedBy":3,"modifiedDate":1369984377779,"facilityId":1,"programId":2,"period":2,"status":"IN_APPROVAL","fullSupplyLineItems":[{"id":1,"modifiedBy":3,"modifiedDate":1369984377782,"rnrId":1,"product":"ACETYL SALICYLIC ACID, TAB 300MG Capsule 300/200/600 mg","productDisplayOrder":4,"productCode":"EM1","productCategory":"Anaesthetics","productCategoryDisplayOrder":4,"roundToZero":false,"packRoundingThreshold":1,"packSize":10,"dosesPerMonth":30,"dosesPerDispensingUnit":10,"dispensingUnit":"Strip","maxMonthsOfStock":3,"fullSupply":true,"quantityReceived":1,"quantityDispensed":1,"beginningBalance":1,"totalLossesAndAdjustments":0,"stockInHand":1,"stockOutDays":0,"newPatientCount":0,"amc":0,"normalizedConsumption":1,"calculatedOrderQuantity":0,"maxStockQuantity":0,"quantityApproved":0,"packsToShip":0,"previousStockInHandAvailable":false,"price":"50.00"},{"id":2,"modifiedBy":3,"modifiedDate":1369984377786,"rnrId":1,"product":"AMOXYCILLIN (TRIHYDRATE), CAP 250MG Capsule 300/200/600 mg","productDisplayOrder":5,"productCode":"EM2","productCategory":"Anaesthetics","productCategoryDisplayOrder":4,"roundToZero":true,"packRoundingThreshold":1,"packSize":10,"dosesPerMonth":30,"dosesPerDispensingUnit":10,"dispensingUnit":"Strip","maxMonthsOfStock":3,"fullSupply":true,"quantityReceived":7,"quantityDispensed":7,"beginningBalance":7,"totalLossesAndAdjustments":0,"stockInHand":7,"stockOutDays":0,"newPatientCount":0,"amc":2,"normalizedConsumption":7,"calculatedOrderQuantity":0,"maxStockQuantity":6,"quantityApproved":0,"packsToShip":0,"previousStockInHandAvailable":false,"price":"50.00"},{"id":3,"modifiedBy":3,"modifiedDate":1369984377789,"rnrId":1,"product":"BENZATHINE BENZYL PENICILLIN , 2.4MU, PWD FOR INJ Capsule 300/200/600 mg","productDisplayOrder":5,"productCode":"EM3","productCategory":"Anaesthetics","productCategoryDisplayOrder":4,"roundToZero":false,"packRoundingThreshold":1,"packSize":10,"dosesPerMonth":30,"dosesPerDispensingUnit":10,"dispensingUnit":"Strip","maxMonthsOfStock":3,"fullSupply":true,"quantityReceived":4,"quantityDispensed":4,"beginningBalance":4,"totalLossesAndAdjustments":0,"stockInHand":4,"stockOutDays":0,"newPatientCount":0,"amc":1,"normalizedConsumption":4,"calculatedOrderQuantity":0,"maxStockQuantity":3,"quantityApproved":0,"packsToShip":0,"previousStockInHandAvailable":false,"price":"50.00"}],"nonFullSupplyLineItems":[],"submittedDate":1369984328023,"comments":[]}}

### HTTP Responses

- **200 OK** - All Indicates that the specified action was successfully completed.
- **401 Unauthorized** - Raised when the username-password combination incorrect.
- **400 Invalid data** - Indicates invalid requisitionId.
- **500 Internal Server Error** - Indicates that the server encountered an error while attempting to execute the desired action.
