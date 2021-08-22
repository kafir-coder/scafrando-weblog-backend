# create post usecase

> ## Caso de sucesso

1. ✅ Recebe uma requisição do tipo **POST** na rota **/api/posts**
2. ✅ Valida se a requisição foi feita por um **admin**
3. ✅ validate the incomming data
   -- request body shouldn't be empty
   -- request body shouldn't be imcompleted
   -- body length mustn't be greater than 2kb
4. ✅ send the body to a highlight script analyzer
5. ✅ **stores** the object in a mongodb collection
6. ✅ returns **201** with the new post

> ## Exceções

1. ✅ returns error **404** if the endpoint doesn't exists
2. ✅ returns error **403** if the user isn't a **admin**
3. ✅ returns error **400** if the validate phase wasn't satisfied
4. ✅ returns **400** if something unexpected happened in the server
