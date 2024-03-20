<HTML>
  <Body> 
<script type='text/javascript'>
    function initEmbeddedMessaging() {
        try {
            embeddedservice_bootstrap.settings.language = 'en-US'; // For example, enter 'en' or 'en-US'


    
        
        window.addEventListener("onEmbeddedMessagingReady", () => {
            console.log("Received the onEmbeddedMessagingReady event…");
            embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ 
            "PlatformUserEmail" : "yose.505@gmail.com" , 
            "PlatformUserType" : "Borrower",
            "PlatformUserID" : "45345345345" ,
            "PlatformUserFirstName" : "Yosef",
            "PlatformUserLastName" : "Hasan",
            "PlatformUserLanguage" : "Arabic"}
            );
        });




            embeddedservice_bootstrap.init(
                '00D8d00000Az0S2',
                'Platform_Web_Chat',
                'https://arat.my.site.com/ESWPlatformWebChat1707284468867',
                {
                    scrt2URL: 'https://arat.my.salesforce-scrt.com'
                }
            );
        } catch (err) {
            console.error('Error loading Embedded Messaging: ', err);
        }
    };
 </Body>
 </HTML>
