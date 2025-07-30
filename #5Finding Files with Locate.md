![alt text](Linux.jpg)

# Finding Files with Locate using Linux

In this section we are going to learn to use locate command to find files within Linux.

# ```locate```

The **locate** command helps us to find files in the Linux System.
For example let's say I am looking for a file name passwd. As you can see the result matching **passwd** is huge. 

The advantage of locate is that it works fast but the disadvantage is that it is poor to filter unwanted results. **locate** command is not efficient if you are looking for a particular file.
```
┌──(kali㉿kali)-[~]
└─$ locate passwd
/etc/passwd
/etc/passwd-
/etc/alternatives/vncpasswd
/etc/alternatives/vncpasswd.1.gz
/etc/pam.d/chpasswd
/etc/pam.d/passwd
/etc/security/opasswd
/usr/bin/autopasswd
/usr/bin/expect_autopasswd
/usr/bin/expect_mkpasswd
/usr/bin/expect_tkpasswd
/usr/bin/gpasswd
/usr/bin/grub-mkpasswd-pbkdf2
/usr/bin/htpasswd
/usr/bin/impacket-changepasswd
/usr/bin/impacket-smbpasswd
/usr/bin/ldappasswd
/usr/bin/mkpasswd
/usr/bin/mosquitto_passwd
/usr/bin/passwd
/usr/bin/smbpasswd
/usr/bin/tightvncpasswd
/usr/bin/tkpasswd
/usr/bin/vncpasswd
/usr/lib/python3/dist-packages/impacket/krb5/kpasswd.py
/usr/lib/python3/dist-packages/impacket/krb5/__pycache__/kpasswd.cpython-311.pyc
/usr/lib/tmpfiles.d/passwd.conf
/usr/lib/x86_64-linux-gnu/samba/libsmbpasswdparser-private-samba.so.0
/usr/sbin/chgpasswd
/usr/sbin/chpasswd
/usr/sbin/sampasswd
/usr/sbin/update-passwd
/usr/share/base-passwd
/usr/share/awk/ns_passwd.awk
/usr/share/awk/passwd.awk
/usr/share/base-passwd/group.master
/usr/share/base-passwd/passwd.master
/usr/share/bash-completion/completions/chpasswd
/usr/share/bash-completion/completions/gpasswd
/usr/share/bash-completion/completions/grub-mkpasswd-pbkdf2
/usr/share/bash-completion/completions/htpasswd
/usr/share/bash-completion/completions/ldappasswd
/usr/share/bash-completion/completions/mkpasswd
/usr/share/bash-completion/completions/passwd
/usr/share/bash-completion/completions/smbpasswd
/usr/share/doc/base-passwd
/usr/share/doc/passwd
/usr/share/doc/tightvncpasswd
/usr/share/doc/base-passwd/README
/usr/share/doc/base-passwd/changelog.gz
/usr/share/doc/base-passwd/copyright
/usr/share/doc/base-passwd/users-and-groups.html
/usr/share/doc/base-passwd/users-and-groups.txt.gz
/usr/share/doc/gawk/examples/lib/ns_passwd.awk
/usr/share/doc/gawk/examples/lib/passwdawk.in
/usr/share/doc/libnet-ssleay-perl/examples/passwd-cb.pl
/usr/share/doc/metasploit-framework/modules/auxiliary/scanner/http/synology_forget_passwd_user_enum.md
/usr/share/doc/metasploit-framework/modules/exploit/linux/http/qnap_qcenter_change_passwd_exec.md
/usr/share/doc/metasploit-framework/modules/post/osx/gather/apfs_encrypted_volume_passwd.md
/usr/share/doc/passwd/NEWS.Debian.gz
/usr/share/doc/passwd/README.Debian
/usr/share/doc/passwd/TODO.Debian
/usr/share/doc/passwd/changelog.Debian.gz
/usr/share/doc/passwd/changelog.gz
/usr/share/doc/passwd/copyright
/usr/share/doc/passwd/examples
/usr/share/doc/passwd/examples/passwd.expire.cron
/usr/share/doc/python-odf-doc/examples/passwd-as-ods.py
/usr/share/doc/python-odf-doc/examples/passwd-as-odt.py
/usr/share/doc/python3-impacket/examples/changepasswd.py
/usr/share/doc/python3-impacket/examples/smbpasswd.py
/usr/share/doc/tightvncpasswd/changelog.Debian.gz
/usr/share/doc/tightvncpasswd/changelog.gz
/usr/share/doc/tightvncpasswd/copyright
/usr/share/doc-base/base-passwd.users-and-groups
/usr/share/lintian/overrides/base-passwd
/usr/share/lintian/overrides/passwd
/usr/share/man/cs/man1/gpasswd.1.gz
/usr/share/man/cs/man5/passwd.5.gz
/usr/share/man/de/man1/gpasswd.1.gz
/usr/share/man/de/man1/passwd.1.gz
/usr/share/man/de/man5/passwd.5.gz
/usr/share/man/de/man8/chgpasswd.8.gz
/usr/share/man/de/man8/chpasswd.8.gz
/usr/share/man/de/man8/update-passwd.8.gz
/usr/share/man/es/man8/update-passwd.8.gz
/usr/share/man/fr/man1/gpasswd.1.gz
/usr/share/man/fr/man1/passwd.1.gz
/usr/share/man/fr/man5/passwd.5.gz
/usr/share/man/fr/man8/chgpasswd.8.gz
/usr/share/man/fr/man8/chpasswd.8.gz
/usr/share/man/fr/man8/update-passwd.8.gz
/usr/share/man/hu/man1/gpasswd.1.gz
/usr/share/man/hu/man1/passwd.1.gz
/usr/share/man/hu/man5/passwd.5.gz
/usr/share/man/it/man1/gpasswd.1.gz
/usr/share/man/it/man1/passwd.1.gz
/usr/share/man/it/man5/passwd.5.gz
/usr/share/man/it/man8/chgpasswd.8.gz
/usr/share/man/it/man8/chpasswd.8.gz
/usr/share/man/ja/man1/gpasswd.1.gz
/usr/share/man/ja/man1/passwd.1.gz
/usr/share/man/ja/man5/passwd.5.gz
/usr/share/man/ja/man8/chpasswd.8.gz
/usr/share/man/ja/man8/update-passwd.8.gz
/usr/share/man/ko/man5/passwd.5.gz
/usr/share/man/man1/expect_mkpasswd.1.gz
/usr/share/man/man1/gpasswd.1.gz
/usr/share/man/man1/grub-mkpasswd-pbkdf2.1.gz
/usr/share/man/man1/htpasswd.1.gz
/usr/share/man/man1/ldappasswd.1.gz
/usr/share/man/man1/mkpasswd.1.gz
/usr/share/man/man1/mosquitto_passwd.1.gz
/usr/share/man/man1/openssl-passwd.1ssl.gz
/usr/share/man/man1/passwd.1.gz
/usr/share/man/man1/passwd.1ssl.gz
/usr/share/man/man1/tightvncpasswd.1.gz
/usr/share/man/man1/vncpasswd.1.gz
/usr/share/man/man3/passwd2des.3.gz
/usr/share/man/man5/passwd.5.gz
/usr/share/man/man5/smbpasswd.5.gz
/usr/share/man/man8/chgpasswd.8.gz
/usr/share/man/man8/chpasswd.8.gz
/usr/share/man/man8/sampasswd.8.gz
/usr/share/man/man8/smbpasswd.8.gz
/usr/share/man/man8/update-passwd.8.gz
/usr/share/man/pl/man8/update-passwd.8.gz
/usr/share/man/pt_BR/man1/gpasswd.1.gz
/usr/share/man/pt_BR/man5/passwd.5.gz
/usr/share/man/ru/man1/gpasswd.1.gz
/usr/share/man/ru/man1/passwd.1.gz
/usr/share/man/ru/man5/passwd.5.gz
/usr/share/man/ru/man8/chgpasswd.8.gz
/usr/share/man/ru/man8/chpasswd.8.gz
/usr/share/man/ru/man8/update-passwd.8.gz
/usr/share/man/sv/man1/passwd.1.gz
/usr/share/man/sv/man5/passwd.5.gz
/usr/share/man/tr/man1/passwd.1.gz
/usr/share/man/tr/man5/passwd.5.gz
/usr/share/man/uk/man1/gpasswd.1.gz
/usr/share/man/uk/man1/passwd.1.gz
/usr/share/man/uk/man5/passwd.5.gz
/usr/share/man/uk/man8/chgpasswd.8.gz
/usr/share/man/uk/man8/chpasswd.8.gz
/usr/share/man/zh_CN/man1/gpasswd.1.gz
/usr/share/man/zh_CN/man1/passwd.1.gz
/usr/share/man/zh_CN/man5/passwd.5.gz
/usr/share/man/zh_CN/man8/chgpasswd.8.gz
/usr/share/man/zh_CN/man8/chpasswd.8.gz
/usr/share/man/zh_TW/man5/passwd.5.gz
/usr/share/man/zh_TW/man8/chpasswd.8.gz
/usr/share/metasploit-framework/lib/rex/post/meterpreter/extensions/priv/passwd.rb
/usr/share/metasploit-framework/lib/rex/post/meterpreter/ui/console/command_dispatcher/priv/passwd.rb
/usr/share/metasploit-framework/modules/auxiliary/scanner/http/bmc_trackit_passwd_reset.rb
/usr/share/metasploit-framework/modules/auxiliary/scanner/http/synology_forget_passwd_user_enum.rb
/usr/share/metasploit-framework/modules/exploits/linux/http/efw_chpasswd_exec.rb
/usr/share/metasploit-framework/modules/exploits/linux/http/piranha_passwd_exec.rb
/usr/share/metasploit-framework/modules/exploits/linux/http/qnap_qcenter_change_passwd_exec.rb
/usr/share/metasploit-framework/modules/exploits/unix/ssh/tectia_passwd_changereq.rb
/usr/share/metasploit-framework/modules/post/osx/gather/apfs_encrypted_volume_passwd.rb
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/httpclient-2.8.3/test/htpasswd
/usr/share/metasploit-framework/vendor/bundle/ruby/3.1.0/gems/webrick-1.8.1/lib/webrick/httpauth/htpasswd.rb
/usr/share/nmap/scripts/http-passwd.nse
/usr/share/python-odf/examples/passwd-as-ods.py
/usr/share/python-odf/examples/passwd-as-odt.py
/usr/share/ri/3.1.0/system/Etc/passwd-c.ri
/usr/share/rubygems-integration/all/gems/webrick-1.8.1/lib/webrick/httpauth/htpasswd.rb
/usr/share/vim/vim91/ftplugin/passwd.vim
/usr/share/vim/vim91/syntax/passwd.vim
/usr/share/weevely/modules/audit/etcpasswd.py
/usr/share/whatweb/plugins/htpasswd.rb
/usr/share/zsh/functions/Completion/Linux/_gpasswd
/var/lib/dpkg/alternatives/vncpasswd
/var/lib/dpkg/info/base-passwd.list
/var/lib/dpkg/info/base-passwd.md5sums
/var/lib/dpkg/info/base-passwd.postinst
/var/lib/dpkg/info/base-passwd.postrm
/var/lib/dpkg/info/base-passwd.preinst
/var/lib/dpkg/info/base-passwd.templates
/var/lib/dpkg/info/passwd.conffiles
/var/lib/dpkg/info/passwd.list
/var/lib/dpkg/info/passwd.md5sums
/var/lib/dpkg/info/passwd.postinst
/var/lib/dpkg/info/passwd.postrm
/var/lib/dpkg/info/passwd.preinst
/var/lib/dpkg/info/passwd.prerm
/var/lib/dpkg/info/tightvncpasswd.list
/var/lib/dpkg/info/tightvncpasswd.md5sums
/var/lib/dpkg/info/tightvncpasswd.postinst
/var/lib/dpkg/info/tightvncpasswd.prerm
```

As demonstrated above that results produced by using **locate** utility can be hard to filter through so we can use the **piping** along with **grep** command to filter our search for a specific file.

Let's say we are looking for all files with an extension **.txt**. We need to use **--all** switch with **locate** command and use the asterisk symbol before *.txt to search all files having the extension mentioned.

```
┌──(kali㉿kali)-[~]
└─$ locate /etc "*.txt"
/etc/X11/rgb.txt
/etc/arp-scan/mac-vendor.txt
/etc/java-17-openjdk/security/policy/README.txt
/etc/java-23-openjdk/security/policy/README.txt
/etc/unicornscan/oui.txt
/etc/unicornscan/ports.txt
```

If you want to find out the number of matches to our searching criteria use the **-c** switch with **locate** command as shown below.

You can also user **-i** switch with **locate** command to ommit case sensitivity.
```
┌──(kali㉿kali)-[~]
└─$ locate /etc --all -c "*.txt"
6
```

