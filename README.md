# OperationQueueAndDispatchSwift

## HW: 
1. Создать свой протокол по работе с данными, там должны быть методы для сохранение моделей, получения моделей, поиска моделей по названию или id. Добавить класс менеджер, который будет реализовывать протокол по работе с данными.  
Ваш класс должен быть синглтоном(загуглить, как в swift 3 создать синглтон).   
2. Каждая операция должна иметь синхронную и асинхронную версию.   
(прим: syncSave(model: Model) asyncSave(model: Model) ) 
3. Асинхронные методы должны иметь completionBlock, в котором вы будете возвращать результат сохранения, получения, поиска.  
4. Для каждой асинхронной операции (сохранение, получение, поиск) должны быть созданы свои OperationQueue и соотвественно вы используете нужную вам очередь добавляя туда те или иные действия и выполняя все асинхронно.  
5. Внутри ваш менеджер данных должен работать пока с  массивым данных ваших новостей, т.е. в него вы сохраняете данные и из него вытаскиваете данные (при поиске модели), или возвращаете этот массив при запросе на все модели.   
6. Используя реализацию менеджера, вывести все записи вашей стены с новостями из этого менеджера.   
7. При добавлении новой записи сохраняете теперь ее через ваш менеджер асинхронно, а затем, асинхронно запрашиваете все данные из менеджера и обновляете таблицу. В итоге ваша новость должна появится на стене.  
8. Не забудьте обновить pullToRefresh этой таблицы с новостями, чтобы тоже работало с вашим менеджером данных.
8. + где нибудь вызывать метод для поиска по названию или id, чтобы показать, что синхронная/асинхронная функция работает.  

## Полезные ссылки: 

https://habrahabr.ru/post/335756/ 
http://swiftbook.ru/content/tutorials/grand-central-dispatch-part1
https://medium.com/ios-recipes-ru/всё-о-многопоточности-в-swift-часть-1-настоящее-f0b4d5718877
