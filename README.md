

DeepFuzzer is a fuzzer which combines qualified seed generation, balanced seed selection, hybrid seed mutation and automatic fuzzing environment configuration.

DeepFuzzer is an extension of AFL which is written and maintained by Michal Zalewski <[lcamtuf@google.com](mailto:lcamtuf@google.com)>, so its basic usage is like AFL, which can be found in http://lcamtuf.coredump.cx/afl/.  

To generate high-quality seeds, please use the tool in seed_generation directory. Besides that, if you want to open the balanced seed selection, please add the -F option. And you can also use –D option to open the hybrid seed mutation. We also supply the –P option  to open power schedule, this is another optimization for AFL to calculate the mutation times of a seed. These functions are closed in default, and you can combine them as you like. We believe that in most cases, opening all of them  is the best option. 