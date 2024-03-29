Configurable Attachment Alert
==========

This Zimlet alerts you when your forget to attach the attachment when sending an email message.

The Zimlet will search for keywords in your message (for example, "attach" or "attachment"). 

And if the keywords exist in your outgoing message, the Zimlet will confirm that at least
one attachment exists before sending. If no attachments exist, an alert dialog is presented.

This is a fork from:
https://github.com/Zimbra-Community/adopted/tree/master/com_zimbra_attachmentalert

This Zimlet is supported with Zimbra version 8.7.11 and above and is tested on 8.8.15 and 9.0.

This version allows you to optionally configure the keywords to look for in
your email message. This way you can write emails in various languages and
still be able to get the attachment alert.

Screenshot: https://raw.githubusercontent.com/Zimbra-Community/attachmentalert-zimlet/master/screenshot.png

Screenshot: https://raw.githubusercontent.com/Zimbra-Community/attachmentalert-zimlet/master/screenshot-preferences.png

========================================================================

### Installing

    su zimbra
    cd /tmp
    rm tk_barrydegraaff_attachmentalert*
    wget https://github.com/Zimbra-Community/attachmentalert-zimlet/releases/download/0.6/tk_barrydegraaff_attachmentalert.zip
    zmzimletctl deploy tk_barrydegraaff_attachmentalert.zip
    (wait 15 minutes for the deploy to propagate; or zmprov fc all && zmmailboxdctl restart)

========================================================================


### License

Copyright (C) 2015-2021 Barry de Graaff
The MIT License

Copyright (C) 2013, 2014, 2015 Dennis Ploeger
The MIT License

Copyright (C) 2005, 2006, 2007, 2008, 2009, 2010 Zimbra, Inc.
The contents of this file are subject to the Zimbra Public License
Version 1.3 ("License")
