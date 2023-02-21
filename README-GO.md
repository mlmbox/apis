# go-genproto

```bash
export MLMBOX_API_PATH="$HOME/go/src/github.com/mlmbox/apis"

protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/bot/processing/v1/processing.proto

protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/account.proto=mlmbox/type/account mlmbox/type/account.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/agent.proto=mlmbox/type/agent mlmbox/type/agent.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/asset.proto=mlmbox/type/asset mlmbox/type/asset.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/bonus.proto=mlmbox/type/bonus mlmbox/type/bonus.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/confirmation.proto=mlmbox/type/confirmation mlmbox/type/confirmation.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/farming.proto=mlmbox/type/farming mlmbox/type/farming.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/google_authenticator.proto=mlmbox/type/google_authenticator mlmbox/type/google_authenticator.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/limit.proto=mlmbox/type/limit mlmbox/type/limit.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/locale.proto=mlmbox/type/locale mlmbox/type/locale.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/payment.proto=mlmbox/type/payment mlmbox/type/payment.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/plan.proto=mlmbox/type/plan mlmbox/type/plan.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/relationship.proto=mlmbox/type/relationship mlmbox/type/relationship.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/session.proto=mlmbox/type/session mlmbox/type/session.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/sort.proto=mlmbox/type/sort mlmbox/type/sort.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/time_point.proto=mlmbox/type/time_point mlmbox/type/time_point.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/type/wallet.proto=mlmbox/type/wallet mlmbox/type/wallet.proto

protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/account/v1/account.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/asset/v1/asset.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/auth/v1/auth.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/confirmation/v1/confirmation.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/confirmation/v1/confirmation_guest.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/farming/v1/farming.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/finance/v1/wallet.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/locale/v1/locale.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/network/v1/network.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/plan/v1/plan.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/client/session/v1/session.proto

protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/local/type/access_token.proto=mlmbox/local/type/access_token mlmbox/local/type/access_token.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/local/type/account.proto=mlmbox/local/type/account mlmbox/local/type/account.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/local/type/asset.proto=mlmbox/local/type/asset mlmbox/local/type/asset.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/local/type/confirmation.proto=mlmbox/local/type/confirmation mlmbox/local/type/confirmation.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/local/type/google_authenticator.proto=mlmbox/local/type/google_authenticator mlmbox/local/type/google_authenticator.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=Mmlmbox/local/type/session.proto=mlmbox/local/type/session mlmbox/local/type/session.proto

protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/account/account.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/asset/asset.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/confirmation/confirmation.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/finance/wallet.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/google_authenticator/google_authenticator.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/locale/locale.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/plan/plan.proto
protoc -I $MLMBOX_API_PATH --go_out=. --go_opt=paths=source_relative --go-grpc_out=. --go-grpc_opt=paths=source_relative mlmbox/local/session/session.proto
```
