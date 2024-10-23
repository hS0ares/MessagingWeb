<html>
<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">    
<head></head>
<body>
<script type='text/javascript'>
    
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'pt_BR'; // For example, enter 'en' or 'en-US'
    
            window.addEventListener("onEmbeddedMessagingReady", e => {
                //var browserInfo = getBrowserInfo();
                //embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({"CPF__c": "77189874267"});
                //embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({"CaseId": "500bm00000CRf13AAD"});
                
            	embeddedservice_bootstrap.userVerificationAPI.setIdentityToken({
                	identityTokenType : "JWT",
                	identityToken :"eyJraWQiOiIxMjM0NSIsImFsZyI6IlJTMjU2In0.eyJpc3MiOiJ0ZXN0SXNzdWVyIiwic3ViIjoidXNlcjEiLCJleHAiOjE3Mjk2NTk3MDUsImlhdCI6MTcyOTY1MzcwNX0.OiqQ9_AR3Dhtyr-1T0KZOEI_qfKvYNACgkdePg0rrqSCG1DbS3LoKUu1VzhiXv8G1CqL1KBVE-yagXQ0I8Cc5dccLYoh4DXtdur3UI-1O4OF-I3cNl3PEeossF954VsoSUoCI5HNv1OtKry-TeDZJOPX4RWAjK6QLSLuTyI4KpgyrDePSvmugzz1c8KIAbgij0lVRy7cgsAXNxCp3-fUMh2EgsLiTvS-Z0xeJlzXGrUJKY4XT8hMhfhfQow7c3I6bpOY1RHTyrENNhSmx0UNiNI7MtLtx-V4LFEFUX6n8AeGPsTE--Vc57NgbK7nagbEoMJjef2qHUPP84fzWaOUVQ"
            	}); 
            
                console.log("Received the onEmbeddedMessagingReady event.");
            });    
        
            embeddedservice_bootstrap.init(
                '00Dbm0000084LF9',
                'Web_Chat',
                'https://valtech-26e-dev-ed.develop.my.site.com/ESWWebChat1723842704538',
                {
                    scrt2URL: 'https://valtech-26e-dev-ed.develop.my.salesforce-scrt.com'
                }
            );
        } catch (err) {
            console.error('Error loading Embedded Messaging: ', err);
        }
    };

</script>
<script type='text/javascript' src='https://valtech-26e-dev-ed.develop.my.site.com/ESWWebChat1723842704538/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>


<h3>Teste chat</h3>
</body>
</html>
