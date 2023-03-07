# go-genproto

```bash
export MLMBOX_API_PATH="$HOME/go/src/github.com/mlmbox/apis"


protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/account.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/agent.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/asset.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/bonus.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/confirmation.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/farming.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/google_authenticator.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/limit.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/locale.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/payment.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/relationship.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/session.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/sort.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/time_point.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/type/wallet.proto

protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/account/v1/account.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/asset/v1/asset.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/auth/v1/auth.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/confirmation/v1/confirmation.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/confirmation/v1/confirmation_guest.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/farming/v1/farming.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/finance/v1/wallet.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/google_authenticator/v1/google_authenticator.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/locale/v1/locale.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/network/v1/network.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated mlmbox/client/session/v1/session.proto

protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/any.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/api.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/descriptor.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/duration.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/empty.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/field_mask.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/source_context.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/struct.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/timestamp.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/type.proto
protoc -I=$MLMBOX_API_PATH --dart_out=grpc:lib/src/generated google/protobuf/wrappers.proto
```
