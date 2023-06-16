![[Pasted image 20230607134108.png]]

#keystore
```
keytool -exportcert -alias YOUR_RELEASE_KEY_ALIAS -keystore YOUR_RELEASE_KEY_PATH | openssl sha1 -binary | openssl base64
```
```
keytool -list -v -keystore taptap.keystore
```
# 知识点
## provider
注册provider，在AndroidManifest.xml文件< application>< /application>标签中