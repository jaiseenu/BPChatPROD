<!DOCTYPE html>
<html lang="en">
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1">
  <title>Embedded Messaging</title>
</head>

<body>
  <script type="text/javascript">
    // Get details from the URL
    function getDetails() {
      const urlParams = new URLSearchParams(window.location.search);
      // Important:
      // - Field API names are case-sensitive and must exactly match the configuration in Salesforce.
      // - Do not rename or modify existing parameter keys.
      // - If you need to include additional fields, ensure they are first configured in Salesforce before adding them here.
      const data = {
        Loan_ID: urlParams.get('loanId'),
        Contact_ID: urlParams.get('contactId'),
        Page_Info: urlParams.get('pageInfo'),
        Device_Type: urlParams.get('deviceType'),
        DPD: urlParams.get('dpd'),
        Session_ID: urlParams.get('sessionId')
      };
      console.log("data:", data);
      return data;
    }

    // Start the chat and set prechat fields
    async function startChat() {
      try {
        console.log("Starting chat...");
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields(getDetails());
        const success = await embeddedservice_bootstrap.utilAPI.launchChat();
        console.log("LAUNCH SUCCESS:", success);
      } catch (error) {
        console.error("LAUNCH ERROR:", error);
      } finally {
        console.log("LAUNCH FINISHED");
      }
    }

    // Initialize Embedded Messaging
    async function initEmbeddedMessaging() {
      try {
        console.log("##embeddedservice_bootstrap:", embeddedservice_bootstrap);
        console.log("##embeddedservice_bootstrapsettings:", embeddedservice_bootstrap.settings);
        embeddedservice_bootstrap.settings.language = 'en_US';
        embeddedservice_bootstrap.settings.enableUserInputForConversationWithBot = true;


        // When user manually clicks the chat button
        window.addEventListener("onEmbeddedMessagingButtonClicked", () => {
          console.log("onEmbeddedMessagingButtonClicked event received");
          embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields(getDetails());
        });

        window.addEventListener("onEmbeddedMessagingButtonCreated", () => {
          console.log("onEmbeddedMessagingButtonCreated event received");
          console.log("##embeddedservice_bootstrapCREATE:", embeddedservice_bootstrap);
          console.log("##embeddedservice_bootstrapsettingsCREATE:", embeddedservice_bootstrap.settings);
        });

        // Initialize Embedded Messaging
       embeddedservice_bootstrap.init(
				'00Dj0000001oqQP',
				'Borrower_Portal',
				'https://pflms.my.site.com/ESWBorrowerPortal1764600240865',
				{
					scrt2URL: 'https://pflms.my.salesforce-scrt.com'
				}
			);

      } catch (error) {
        console.error("Error initializing Embedded Messaging:", error);
      }
    }
  </script>

  <!-- Salesforce Embedded Messaging Bootstrap -->
  <script type='text/javascript' src='https://pflms.my.site.com/ESWBorrowerPortal1764600240865/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>
</body>
</html>
