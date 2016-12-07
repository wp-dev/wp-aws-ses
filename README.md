#Amazon SES DKIM Mailer

This is a clone of the [original Wordpress plugin](https://wordpress.org/plugins/amazon-ses-and-dkim-mailer/) with fixes. 

This plugin which was originally created by Anatta (Nick Murray), adds Amazon SES, DKIM and third party SMTP capability to the WordPress mailing system for outgoing e-mails. It is based on the configure-smtp plugin v3.1 by coffee2code and the Amazon SES class for PHPMailer by Titon Barua.

The plugin provides the ability to configure the following:

##Amazon SES

- Amazon AWS access key and secret key
- Amazon SES Validated 'From:' address
- 'From:' Sender Name

###DKIM:

- DKIM private key
- DKIM private key password
- DKIM domain
- DKIM selector

###SMTP (if not using SES):

- SMTP host name
- SMTP port number
- If SMTPAuth (authentication) should be used.
- SMTP username
- SMTP password
- SMTP connection (ssl or tls)

Regardless of whether Amazon SES or SMTP is enabled, the plugin provides you the ability to use the name and e-mail of the 'From:' field for all outgoing e-mails and to enable DKIM signing if your web host or server mail service does not provide DKIM.

Two test buttons are also available that allows you to send a test e-mail to yourself and to a DKIM checking service to validate everything has been properly configured.

Additional Links: [Plugin Homepage](https://wordpress.org/plugins/amazon-ses-and-dkim-mailer/)

###To do:

- Incorporate Amazon SES stats reporting
- Implement failover to SMTP once SES quota is reached, or 
- SES error code received
- Add simple DKIM key and DNS record generator to plugin homepage
- Update to new version of PHPMailer class