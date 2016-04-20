1.Get token

  endpoint: /api/v1/token-auth 

    Content-Type: application/json
    HTTP Method: POST
    JSON: {"username": "User_name", "password":"Password"}, default user "test" password "test"
    
    $ curl -H "Content-Type: application/json" -d '{"username": "test", "password":"test"}' http://127.0.0.1:5000/api/v1/token-auth
    
    {"token":"eyJhbGciOiJSUzUxMiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE0NjE0NTQ4MjIsImlhdCI6MTQ2MTE5NTYyMiwic3ViIjoiIn0.qOgPF-_CHwiq5zBKVIoz8In-7LaOu0ykltz5aIMTyjDoCT27SfzMH-Br4PSuVXxghnQ0jDGVACc80pGZtOR6yQS-9Dzj_eMGZIEbuEMdwhslJeYiMzN0E33UWlo24j9RxabAsVZZKm1b37wEAOC98KJnYO1IaxtOu8RQmJ72tcLNMjHiX770NOc2vzBpkgDjzOHZIV3WNwU0baqf5Fx0fZ9C2eGZgsVt4-Yq2Vve7zTErwhjZHg6wGCBbaOxW-yCegqtjcbbZTCnOp2htu1_qGArbXbJpPXI0AteWsz7FvHUrJIw40RZffa90TPU7KT6hiJ4iLJjehEetTit_RIUDA"}
    

2 Get message "Hello, World"

  endpoint: /api/v1/hello
    
    Content-Type: application/json
    HTTP Method: GET
    
    $curl -H "Authorization:Bearer eyJhbGciOiJSUzUxMiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE0NjE0NTQ4MjIsImlhdCI6MTQ2MTE5NTYyMiwic3ViIjoiIn0.qOgPF-_CHwiq5zBKVIoz8In-7LaOu0ykltz5aIMTyjDoCT27SfzMH-Br4PSuVXxghnQ0jDGVACc80pGZtOR6yQS-9Dzj_eMGZIEbuEMdwhslJeYiMzN0E33UWlo24j9RxabAsVZZKm1b37wEAOC98KJnYO1IaxtOu8RQmJ72tcLNMjHiX770NOc2vzBpkgDjzOHZIV3WNwU0baqf5Fx0fZ9C2eGZgsVt4-Yq2Vve7zTErwhjZHg6wGCBbaOxW-yCegqtjcbbZTCnOp2htu1_qGArbXbJpPXI0AteWsz7FvHUrJIw40RZffa90TPU7KT6hiJ4iLJjehEetTit_RIUDA" http://127.0.0.1:5000/api/v1/hello

    { "message":"Hello, World!"}
