**_`****`_**# PaymentHub

Configuration
---------------
```sh
#SFTP server
sftp.host=192.168.99.100
sftp.port=2222

sftp.user=foo
sftp.upload.path=/CFR-UAT/InputData/
sftp.download.path=/pmhftp/TempCFR/Outbound/
sftp.ssh.keyfile=nopp
sftp.ssh.passphrase=

#File
file.name.dateformat=yyyyMMdd
file.name.type=TXT
file.name.prefix=TRN_PH_PAY_,TRN_PH_WHT_

#Log4j
log.config.file=log4j.properties
```

Usage command
---------------
```sh
java -Dconfig.file=${config.properties} -jar ${PaymentHub.jar} ${mode}
```
  Use -Dconfig.file=${config.properties} to get your config
	
  Use -jar ${CFR.jar} to get your jarfile to run


