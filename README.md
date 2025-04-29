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
  changed(changed .org one line only, other lines are same):
   > .org $C000 ; $C000から開始
  then build with nesasm.
That is all. Enjoy!
</PRE>
<img src=https://github.com/cobwebkanamachi/nes-helloworld-mapper0/blob/main/hw.jpg><BR>
notice:<BR>
I use this flash cart "レトロダンパー ファミコン用「FCマッパー0 Ver.1 フラッシュカートリッジ」 ゲームバンクウェブドットコム Gamebank-web.com".<BR>
And I use this dumper for read and write cart.レトロダンパー 「FC ダンパー V4.1」 ファミコン Famicom ファミリーコンピュータ(Family Computer) ●USBケーブル(Type-C)50cm付属● RetroDumper<BR>
Sorry that were not kazzo or tuna or raspbery pi.
