# go-genproto

```bash
npm install -g grpc-tools
```

```bash
export MLMBOX_API_PATH="$HOME/go/src/github.com/mlmbox/apis"

protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/account.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/agent.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/asset.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/bonus.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/confirmation.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/farming.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/google_authenticator.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/limit.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/locale.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/payment.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/relationship.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/session.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/sort.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/time_point.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/type/wallet.proto

protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/account/v1/account.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/asset/v1/asset.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/auth/v1/auth.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/confirmation/v1/confirmation.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/confirmation/v1/confirmation_guest.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/farming/v1/farming.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/finance/v1/wallet.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/google_authenticator/v1/google_authenticator.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/locale/v1/locale.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/network/v1/network.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. mlmbox/client/session/v1/session.proto

protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/any.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/api.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/descriptor.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/duration.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/empty.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/field_mask.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/source_context.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/struct.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/timestamp.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/type.proto
protoc -I=$MLMBOX_API_PATH --js_out=import_style=commonjs,binary:. --grpc-web_out=import_style=typescript,mode=grpcwebtext:. google/protobuf/wrappers.proto
```
