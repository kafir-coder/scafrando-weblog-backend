# update post usecase

> ## success case

1. ✅ receives a **PUT** request on route **/api/posts/{post_id}**
2. ✅ validates if the requisition was triggered by a **admin**
3. ✅ validate the incomming data
   -- request body shouldn't be empty
   -- request body shouldn't be imcompleted
   -- body length mustn't be greater than 2kb
4. ✅ **stores** the object in a mongodb collection
5. ✅ returns **200** with the updated post

> ## exceptions

1. ✅ returns error **404** if the endpoint doesn't exists
2. ✅ returns error **403** if the user isn't a **admin**
3. ✅ returns error **400** if the validate phase wasn't satisfied
4. ✅ returns **400** if something unexpected happened in the server
