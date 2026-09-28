
.PHONY: all build test clean check

all: build

build:
	cargo build --all-targets --features all

test:
	cargo test --verbose --features all

check:
	cargo fmt --check && cargo rustc --lib --features all -- -D warnings && cargo check --target x86_64-pc-windows-msvc --all-features

clean:
	cargo clean

.DEFAULT_GOAL := all
