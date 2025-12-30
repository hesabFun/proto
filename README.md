# Ledger Service Protocol Buffers

Protocol buffer definitions for a multi-tenant double-entry accounting ledger service.

## Overview

This repository contains the gRPC service definitions for a ledger system that supports:
- Multi-tenant account management
- Double-entry bookkeeping with journal entries
- Account hierarchies and balances
- Multiple currencies and account types

## Service Definition

**Package**: `ledger.v1`
**Go Package**: `github.com/hesabFun/ledger/gen/go/ledger/v1;ledgerv1`

## Generating Code

### Go
```bash
protoc --go_out=. --go_opt=paths=source_relative \
  --go-grpc_out=. --go-grpc_opt=paths=source_relative \
  ledger/v1/ledger.proto
```

### Other Languages
Refer to the [Protocol Buffers documentation](https://protobuf.dev/) for language-specific generation instructions.

## Proto File Location

`ledger/v1/ledger.proto`