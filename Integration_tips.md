# Paytm
### Resources for dev
 1. https://developer.paytm.com/docs/getting-started/
 2. https://www.androidhive.info/2019/02/android-integrating-paytm-payment-gateway-ecommerce-app/
 3. https://www.blueappsoftware.com/paytm-payment-gateway-integration-android-studio/
 4. https://www.simplifiedcoding.net/paytm-integration-android-example/
 5. https://github.com/Anas73412/Paytm , Video : https://youtu.be/6KsxBK3zWjI
 6. https://github.com/signalarun/Paytm_App_Checksum_Kit_NodeJs
 
### Prerequisite  
 1. Get test credentials from https://dashboard.paytm.com
### Integration Steps for Paytm all-in-one SDK
 1. Get order Id from backend
 2. Get checksum from backend with order id and credentials provided by Paytm backend
    Parameters are :
     MID(Merchant ID from Paytm dashboard), Order Id, Customer ID, Website[From Paytm dashboard], Amount, Channel ID, Callback URL and
     Industry type.
     
     callbackurl -> https://pguat.paytm.com/paytmchecksum/paytmCallback.jsp
 3. Start transaction with all-in-one-sdk using the required parameters in the Paytm documentation along the previously obtained checksum.
     Paytm takes care of communicating with back and completing the transaction
 4. Check transaction status using transaction status API of backend server and this server communicates with Paytm server to get the
    transaction status and returns the status to the app.
    
 
 
 
