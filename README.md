# schoolfond

Если в VScode package main подчеркивается красной волнистой линией и выдает ошибку:

``
Error loading workspace: gopls was not able to find modules in your workspace. When outside of GOPATH, gopls needs to know which modules you are working on. You can fix this by opening your workspace to a folder inside a Go module, or by using a go.work file to specify multiple modules. See the documentation for more information on setting up your workspace: https://github.com/golang/tools/blob/master/gopls/doc/workspace.md
``

...это означает что gopls не может подгрузиться и нужно инициализировать модуль. Если у вас еще нет файла go.mod, выполните команду

```
go mod init имя_вашего_модуля
```

чтобы создать его. В качестве имя_вашего_модуля используйте имя, которое хотите дать вашему модулю, например, можно использовать название вашего проекта.