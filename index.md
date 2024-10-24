<html>
<head></head>
<body>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'pt_BR'; // For example, enter 'en' or 'en-US'
			window.addEventListener("onEmbeddedMessagingReady", () => {
				console.log(
				    "onEmbeddedMessagingReady event"
				);
				embeddedservice_bootstrap.userVerificationAPI.setIdentityToken({
				    identityTokenType: "JWT",
				    identityToken: "eyJraWQiOiIxMjM0NSIsImFsZyI6IlJTMjU2In0.eyJpc3MiOiJ0ZXN0SXNzdWVyIiwic3ViIjoidXNlcjEiLCJleHAiOjE3Mjk2NTk3MDUsImlhdCI6MTcyOTY1MzcwNX0.OiqQ9_AR3Dhtyr-1T0KZOEI_qfKvYNACgkdePg0rrqSCG1DbS3LoKUu1VzhiXv8G1CqL1KBVE-yagXQ0I8Cc5dccLYoh4DXtdur3UI-1O4OF-I3cNl3PEeossF954VsoSUoCI5HNv1OtKry-TeDZJOPX4RWAjK6QLSLuTyI4KpgyrDePSvmugzz1c8KIAbgij0lVRy7cgsAXNxCp3-fUMh2EgsLiTvS-Z0xeJlzXGrUJKY4XT8hMhfhfQow7c3I6bpOY1RHTyrENNhSmx0UNiNI7MtLtx-V4LFEFUX6n8AeGPsTE--Vc57NgbK7nagbEoMJjef2qHUPP84fzWaOUVQ",
				});
			});
			
			embeddedservice_bootstrap.init(
				'00Dbm0000084LF9',
				'ESD_MIAW',
				'https://valtech-26e-dev-ed.develop.my.site.com/ESWESDMIAW1729780055975',
				{
					scrt2URL: 'https://valtech-26e-dev-ed.develop.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://valtech-26e-dev-ed.develop.my.site.com/ESWESDMIAW1729780055975/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

<h3>Teste chat 2</h3>
<img src="chat_agente.jpg" />
</body>
</html>
