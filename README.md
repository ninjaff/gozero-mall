# gozero-mall 

## common 
- add errorx
- add jwt
- add cryptx

## midderware
add PeriodLimit

## env
run etcd redis mysql

### mysql init
- ./docs/add-mysql-user.sql
- ./service/user/model/import-tables.sh
- ./service/product/model/import-tables.sh
- ./service/order/model/import-tables.sh
- ./service/pay/model/import-tables.sh

### redis add rpc auth
`redis-cli -h 127.0.0.1 -p 6379 -a 'shunc!#10010sh' hset rpc:auth:user userapi 6jKNZbEpYGeUMAifz10gOnmoty3TV`

## gen rpc api
- ./service/user/gen-user-rpc.sh
- ./service/user/gen-user-api.sh
- ./service/product/gen-product-rpc.sh
- ./service/product/gen-product-api.sh
- ./service/order/gen-order-rpc.sh
- ./service/order/gen-order-api.sh
- ./service/pay/gen-pay-rpc.sh
- ./service/pay/gen-pay-api.sh

## run
- ./service/user/rpc/run.sh
- ./service/user/api/run.sh
- ./service/product/rpc/run.sh
- ./service/product/api/run.sh
- ./service/order/rpc/run.sh
- ./service/order/api/run.sh
- ./service/pay/rpc/run.sh
- ./service/pay/api/run.sh

## swagger
### feature 
配置 登录验证

### use swagger
- ./service/user/gen-user-swagger.sh
- ./service/user/run-swagger.sh