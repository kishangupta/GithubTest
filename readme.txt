           **** Akamai NetSession Interface  ****

--------
Overview
--------

This file describes the Akamai NetSession Interface.

The Akamai NetSession Interface is a download manager application. It was 
installed on your computer when you downloaded content that uses the service 
to provide secure, high integrity downloads of large files. 

The NetSession Interface supports downloading from a central source and between
peers. When peer-downloading is enabled, your computer can serve as an upload
source for other computers -- without adverse impacts to your computing.
Peer-to-peer downloading can provide faster, more effective downloads. 

The NetSession Interface contains no adware or spyware, is safe and secure,
uses minimal resources, and provides you the ability to manage and control its
actions, including the ability to uninstall it if you do not want it on your
computer.

------------
How It Works
------------

The NetSession Interface does not have a noticeable desktop presence during
downloads, since its work is integrated into the sites or applications that use
the service.

However, there are two interfaces you can use to manage downloads and the
interface itself: admintool and a Control Panel extension.

--------------------------------------------------------------
Windows Control Panel / Mac OS X System Preferences Extension
--------------------------------------------------------------

The Control Panel / System Preferences extension provides you an easy way to
manage NetSession functions, such as starting or stopping the service. The
extension also provides you with a Troubleshooting test you can run to tell you
whether your NetSession Interface is installed correctly and can download
properly.

When installed, the extensions are available:

    On the Windows Control Panel: 
    Akamai NetSession Interface Control Panel. 

    On the Mac, on the System Preferences pane: 
    under Other --> Akamai

Note that with Windows Vista 64-bit, additional steps may be required to view 
the NetSession Control Panel in the Windows Control Panel directory. 
Open the Control Panel, select Additional Options and enable the option 
to View 32- bit control panel items.

------------------------------------------------
admintool and the NetSession Installation Folder
------------------------------------------------

admintool is a command-line utility used to get information about the current
NetSession download activities, to stop or start download sessions, clear the
download cache of all downloads, and uninstall the NetSession Interface.

To see all the commands available to you with admintool:

1) Go to the command line of your computer. You can do this as follows:

   On Windows, select Command Prompt from the Start menu, OR...
   Run on the Start menu, type "cmd" into the Open text box, then click OK.

   On Mac OS X, in the Application -> Utilities folder, double-left click
Terminal. 

2) Go to the Akamai NetSession Interface installation folder. 

   The installation folder location depends on your configuration. Normally, it 
   is found in the following locations, where you would replace 
   <user name> with your user name:

   On Windows XP:
      C:\Documents and Settings\<user name>\Local Settings\Application Data\Akamai

   On Windows Vista and Windows 7:
      C:\Users\<user name>\AppData\Local\Akamai

   On Macintosh OS X:
      /Users/<user name>/Applications/Akamai
 
3) Type the command 

    admintool help

4)  Press the Enter (Return) key

All  admintool commands are run in the same way as admintool help in steps 3)
and 4). 


------------
Uninstalling
------------

Before you uninstall, please note: If you uninstall the service, you will
delete files downloaded to the cache folders under the installation folders. If
you don't want to delete those files, copy or move them to a different folder. 

If you do not have a serious need to uninstall the service, it may be better
not to, since other downloads may require NetSession later. NetSession may be
installed again when you download software or media that uses this service.

Also, the Akamai NetSession Interface is a shared network library that may be
used by multiple applications. It will uninstall correctly only when other
applications using the interface are uninstalled. Other applications may not
perform correctly if they look for but do not find the NetSession Interface. 
For that reason, you should not simply delete the NetSession files.

Uninstalling on Windows
-----------------------

The simplest and preferred method is to use the Add or Remove Programs
application.

1) In the Windows Control Panel, run Add or Remove Programs. 

2) Select Akamai NetSession Interface 

3) Click Change/Remove, then click Yes to confirm your choice.

Windows Alternate Method
------------------------

Alternatively, you may open Windows Explorer, go to the installation folder,
then double-click uninstall.exe.

Uninstalling on Mac OS X
------------------------

The simplest and preferred method is to use the Finder to go to the NetSession installation
folder described above, then double-click the uninstaller app. Confirm your decision.

Mac OS X Alternative Methods
----------------------------

There are two alternative uninstall methods.

The first alternative method also works in Windows, but the methods listed in the Windows section are simpler and
are preferred for that system.

   1) As described in the "admintool" section above, go to the command line, and
then go to the NetSession installation folder.

   2) Type the command:

   admintool uninstall -force
   3) Press the Enter (Return)  key to complete the command.

The Launch Unload Mac OS X Alternative
---------------------------------------

This alternative method may be used, for example, if you deleted admintool
without running the admintool uninstall steps described just above. This
uninstall involves required steps of manually stopping the client, then
removing the installation directory, the automatic startup script, and the
preferences panel.

   1) As described in the "admintool" section above, go to the command line.

   2) Type the following lines, and after typing each line, press the Enter
(Return) key to complete the command:

   launchctl unload ~/Library/LaunchAgents/com.akamai.single-user-client.plist
   rm -rf ~/Applications/Akamai
   rm -rf ~/Library/LaunchAgents/com.akamai.single-user-client.plist
   rm -rf ~/Library/PreferencePanes/AkamaiNetSession.prefPane

   3) If the NetSession client isn't stopped when you have gone through these
steps, restart your computer to complete the operation.

-----------------------------
Further Support & Information 
-----------------------------

The Control Panel / System Preferences extension provides an easy way to
manage many NetSession functions, and it provides help in Troubleshooting
and links to more information. It is described above in the section,
"Windows Control Panel / Mac OS X System Preferences Extension."

For  a FAQ, a user "Bill of Rights" and privacy policy, as well as technical
overview and design principles, visit our Web site at:

   http://www.akamai.com/client

Thank you for using Akamai NetSession Interface. 

Akamai Technologies, Inc.    http://www.akamai.com

                 ****

----------------------------------------
License Information and Acknowledgements
----------------------------------------

Copyright (c) 2008-2012 Akamai Technologies, Inc. All Rights Reserved.

The package of software that includes the Akamai software described above
also includes software from the following projects.

Google Breakpad
---------------
Copyright (c) 2006, Google Inc.
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are
met:

    * Redistributions of source code must retain the above copyright
notice, this list of conditions and the following disclaimer.
    * Redistributions in binary form must reproduce the above
copyright notice, this list of conditions and the following disclaimer
in the documentation and/or other materials provided with the
distribution.
    * Neither the name of Google Inc. nor the names of its
contributors may be used to endorse or promote products derived from
this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

OpenSSL Toolkit
---------------
This product includes software developed by the OpenSSL Project
for use in the OpenSSL Toolkit (http://www.openssl.org/).

/* ====================================================================
 * Copyright (c) 1998-2011 The OpenSSL Project.  All rights reserved.
 *
 * Redistribution and use in source and binary forms, with or without
 * modification, are permitted provided that the following conditions
 * are met:
 *
 * 1. Redistributions of source code must retain the above copyright
 *    notice, this list of conditions and the following disclaimer.
 *
 * 2. Redistributions in binary form must reproduce the above copyright
 *    notice, this list of conditions and the following disclaimer in
 *    the documentation and/or other materials provided with the
 *    distribution.
 *
 * 3. All advertising materials mentioning features or use of this
 *    software must display the following acknowledgment:
 *    "This product includes software developed by the OpenSSL Project
 *    for use in the OpenSSL Toolkit. (http://www.openssl.org/)"
 *
 * 4. The names "OpenSSL Toolkit" and "OpenSSL Project" must not be used to
 *    endorse or promote products derived from this software without
 *    prior written permission. For written permission, please contact
 *    openssl-core@openssl.org.
 *
 * 5. Products derived from this software may not be called "OpenSSL"
 *    nor may "OpenSSL" appear in their names without prior written
 *    permission of the OpenSSL Project.
 *
 * 6. Redistributions of any form whatsoever must retain the following
 *    acknowledgment:
 *    "This product includes software developed by the OpenSSL Project
 *    for use in the OpenSSL Toolkit (http://www.openssl.org/)"
 *
 * THIS SOFTWARE IS PROVIDED BY THE OpenSSL PROJECT ``AS IS'' AND ANY
 * EXPRESSED OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
 * PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE OpenSSL PROJECT OR
 * ITS CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 * SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
 * NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 * STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
 * OF THE POSSIBILITY OF SUCH DAMAGE.
 * ====================================================================
 *
 * This product includes cryptographic software written by Eric Young
 * (eay@cryptsoft.com).  This product includes software written by Tim
 * Hudson (tjh@cryptsoft.com).
 *
 */

Original SSLeay License
-----------------------
/* Copyright (C) 1995-1998 Eric Young (eay@cryptsoft.com)
 * All rights reserved.
 *
 * This package is an SSL implementation written
 * by Eric Young (eay@cryptsoft.com).
 * The implementation was written so as to conform with Netscapes SSL.
 *
 * This library is free for commercial and non-commercial use as long as
 * the following conditions are aheared to.  The following conditions
 * apply to all code found in this distribution, be it the RC4, RSA,
 * lhash, DES, etc., code; not just the SSL code.  The SSL documentation
 * included with this distribution is covered by the same copyright terms
 * except that the holder is Tim Hudson (tjh@cryptsoft.com).
 *
 * Copyright remains Eric Young's, and as such any Copyright notices in
 * the code are not to be removed.
 * If this package is used in a product, Eric Young should be given attribution
 * as the author of the parts of the library used.
 * This can be in the form of a textual message at program startup or
 * in documentation (online or textual) provided with the package.
 *
 * Redistribution and use in source and binary forms, with or without
 * modification, are permitted provided that the following conditions
 * are met:
 * 1. Redistributions of source code must retain the copyright
 *    notice, this list of conditions and the following disclaimer.
 * 2. Redistributions in binary form must reproduce the above copyright
 *    notice, this list of conditions and the following disclaimer in the
 *    documentation and/or other materials provided with the distribution.
 * 3. All advertising materials mentioning features or use of this software
 *    must display the following acknowledgement:
 *    "This product includes cryptographic software written by
 *     Eric Young (eay@cryptsoft.com)"
 *    The word 'cryptographic' can be left out if the rouines from the library
 *    being used are not cryptographic related :-).
 * 4. If you include any Windows specific code (or a derivative thereof) from
 *    the apps directory (application code) you must include an acknowledgement:
 *    "This product includes software written by Tim Hudson (tjh@cryptsoft.com)"
 *
 * THIS SOFTWARE IS PROVIDED BY ERIC YOUNG ``AS IS'' AND
 * ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
 * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
 * ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
 * FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
 * OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 * LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
 * OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
 * SUCH DAMAGE.
 *
 * The licence and distribution terms for any publically available version or
 * derivative of this code cannot be changed.  i.e. this code cannot simply be
 * copied and put under another distribution licence
 * [including the GNU Public Licence.]
 */

zlib
----
Copyright (C) 1995-2010 Jean-loup Gailly and Mark Adler

This software is provided 'as-is', without any express or implied
warranty.  In no event will the authors be held liable for any damages
arising from the use of this software.

Permission is granted to anyone to use this software for any purpose,
including commercial applications, and to alter it and redistribute it
freely, subject to the following restrictions:

1. The origin of this software must not be misrepresented; you must not
   claim that you wrote the original software. If you use this software
   in a product, an acknowledgment in the product documentation would be
   appreciated but is not required.
2. Altered source versions must be plainly marked as such, and must not be
   misrepresented as being the original software.
3. This notice may not be removed or altered from any source distribution.

Jean-loup Gailly
Mark Adler

Boost
-----
Boost Software License - Version 1.0 - August 17th, 2003

Permission is hereby granted, free of charge, to any person or organization
obtaining a copy of the software and accompanying documentation covered by
this license (the "Software") to use, reproduce, display, distribute,
execute, and transmit the Software, and to prepare derivative works of the
Software, and to permit third-parties to whom the Software is furnished to
do so, all subject to the following:

The copyright notices in the Software and this entire statement, including
the above license grant, this restriction and the following disclaimer,
must be included in all copies of the Software, in whole or in part, and
all derivative works of the Software, unless such copies or derivative
works are solely in the form of machine-executable object code generated by
a source language processor.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
DEALINGS IN THE SOFTWARE.

TinyXML
-------
www.sourceforge.net/projects/tinyxml
Original code (2.0 and earlier )copyright (c) 2000-2006 Lee Thomason (www.grinninglizard.com)

This software is provided 'as-is', without any express or implied
warranty. In no event will the authors be held liable for any
damages arising from the use of this software.
 
Permission is granted to anyone to use this software for any
purpose, including commercial applications, and to alter it and
redistribute it freely, subject to the following restrictions:

1. The origin of this software must not be misrepresented; you must
not claim that you wrote the original software. If you use this
software in a product, an acknowledgment in the product documentation
would be appreciated but is not required.

2. Altered source versions must be plainly marked as such, and
must not be misrepresented as being the original software.
 
3. This notice may not be removed or altered from any source
distribution.

INRIA LDPC FEC Implementation
-----------------------------
http://planete-bcast.inrialpes.fr/article.php3?id_article=16

LDPC FEC Licence
This codec is: 
  Copyright (c) 2002-2006 INRIA - All rights reserved. 
  Copyright (c) 1995-2003 by Radford M. Neal

The code coming from Radford M. Neal is distributed under the following licence:
    
    Permission is granted for anyone to copy, use, modify, or distribute these 
    programs and accompanying documents for any purpose, provided this copyright 
    notice is retained and prominently displayed, along with a note saying that 
    the original programs are available from Radford Neal's web page, and note is 
    made of any changes made to these programs. These programs and documents are 
    distributed without any warranty, express or implied. As the programs were 
    written for research purposes only, they have not been tested to the degree 
    that would be advisable in any important application. All use of these programs 
    is entirely at the user's own risk.

The code coming from INRIA is distributed under the GNU/LGPL licence, with the 
following additional requirement:

    This copyright notice must be retained and prominently displayed, along with a 
    note saying that the original programs are available from Vincent Roca's web page, 
    and note is made of any changes made to these programs.

