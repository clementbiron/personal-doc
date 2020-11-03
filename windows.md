# Windows

* Quicklook, quick preview : [https://www.microsoft.com/en-us/p/quicklook/9nv4bs3l1h4s?activetab=pivot:overviewtab](https://www.microsoft.com/en-us/p/quicklook/9nv4bs3l1h4s?activetab=pivot:overviewtab)
* Wox launcher : [http://www.wox.one/](http://www.wox.one/)
* Bulk install Windows apps quickly with Windows Package Manager. : [https://winstall.app/](https://winstall.app/)

### WSL

#### Erreurs

Pas les droits pour écrire un fichier ?

```text
Failed to save 'file.js': Unable to write file (NoPermissions (FileSystemError): Error: EACCES: permission denied, open '/opt/path/to/folder/file.js')
```

Il faut changer les droits de l'utilisateur :

```text
sudo chown -R myuser /path/to/folder
```

