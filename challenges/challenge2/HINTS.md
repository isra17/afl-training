Because we're using ASAN, we need to run this in a slightly different way, see docs/notes_for_asan.txt:

	sudo /afl-*/experimental/asan_cgroups/limit_memory.sh -u fuzzer /afl-*/afl-fuzz -i in -o out -m none ./handshake
