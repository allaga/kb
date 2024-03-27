dd - convert and copy a file

if=FILE
              read from FILE instead of stdin

of=FILE
              write to FILE instead of stdout

bs=BYTES
              read  and  write  up  to  BYTES bytes at a time (default: 512);
              overrides ibs and obs
              
count=N
              copy only N input blocks


dd работает с необраотанными данными (RAW) на самом низком уровне - на уровне секторов жесткого диска. Именно поэтому dd так опасна. Ведь она может запросто взять секторы одного диска и заменить ими секторы другого диска.