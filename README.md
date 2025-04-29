# nes-helloworld-mapper0
tekepen and dumbo's helloworld slightly modified for running on mapper 0 flash cart.
<PRE>
1. base is tekepen(https://tekepen.com/nes/sample.html#samples)'s one.
   https://tekepen.com/nes/sample/helloworld.zip
2. then, overwrite dumbo's one.
   https://dumbo001.hatenablog.com/entry/2023/05/27/155053
   He changed mainly adjust for nesasm(he wrote).
3. slightly mod.
   original:
   > ; 起動
   > .bank 0    ; バンク0 
   > .org $8000 ; $8000から開始
   > ; リセット割り込み
   > Reset:
  changed:
   > .org $C000 ; $C000から開始
  then build with nesasm.
That is all. Enjoy!
</PRE>
