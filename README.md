# Compile and Run
emcc test.c -s WASM=1 -s SIDE_MODULE=1 -O1 -s EXPORTED_FUNCTIONS='["_add"]' -o test.wasm 
emrun --no_browser --port 8080 . &