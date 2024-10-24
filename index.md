<html>
<head></head>
<body>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'pt_BR'; // For example, enter 'en' or 'en-US'

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
</body>
</html>
