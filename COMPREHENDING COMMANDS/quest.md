# Filestorm Quest

## My Solve:
Just Do as instucted by pwn.college

*Flag:* pwn.college{I_iza9DbnpNi5oZNeV8OV-3heZ7.QX5IDO0wCOwMzNzEzW}

bash \
hacker@commands\~an-epic-filesystem-quest:\~$ cd /    
hacker@commands\~an-epic-filesystem-quest:/$ ls -a                    
.   .dockerenv  bin   challenge  etc   home  lib32  libx32  mnt  opt   root  sbin  sys  usr                       
..  BLUEPRINT   boot  dev        flag  lib   lib64  media   nix  proc  run   srv   tmp  var                   
hacker@commands\~an-epic-filesystem-quest:/$ cat BLUEPRINT                 
Yahaha, you found me!                    
The next clue is in: /opt/pwndbg/.venv/lib/python3.8/site-packages/pip/_vendor/truststore                                          

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.                        
hacker@commands~an-epic-filesystem-quest:/$ ls -a /opt/pwndbg/.venv/lib/python3.8/site-packages/pip/_vendor/truststore   
.  ..  .DOSSIER  __init__.py  __pycache__  _api.py  _macos.py  _openssl.py  _ssl_constants.py  _windows.py  py.typed                  
hacker@commands\~an-epic-filesystem-quest:/$ cd /opt/pwndbg/.venv/lib/python3.8/site-packages/pip/_vendor/truststore                    
hacker@commands\~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/pip/_vendor/truststore$ cat .DOSSIER                             
Congratulations, you found the clue!                    
The next clue is in: /usr/lib/python3/dist-packages/sympy/tensor/array                           
                                            
The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.                                   
hacker@commands\~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/pip/_vendor/truststore$ cd /usr/lib/python3/dist-packages/sympy/tensor/array               
hacker@commands\~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/tensor/array$ ls -a                
.   SNIPPET      __pycache__             arrayop.py           mutable_ndim_array.py  sparse_ndim_array.py             
..  __init__.py  array_comprehension.py  dense_ndim_array.py  ndim_array.py          tests              
hacker@commands\~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/tensor/array$ cat  SNIPPET                     
Congratulations, you found the clue!                  
The next clue is in: /usr/share/doc/libwayland-cursor0                         
                                                          
The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.               
hacker@commands\~an-epic-filesystem-quest:/usr/lib/python3/dist-packages/sympy/tensor/array$ cd /usr/share/doc/libwayland-cursor0                          
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ ls -a                   
.  ..  .GIST  changelog.Debian.gz  copyright                      
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cat .GIST               
Congratulations, you found the clue!           
The next clue is in: /opt/linux/linux-5.4/tools/lib/api                                   

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!                 
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ ls -a  /opt/linux/linux-5.4/tools/lib/api                      
.  ..  Build  Makefile  NOTE-TRAPPED  cpu.c  cpu.h  debug-internal.h  debug.c  debug.h  fd  fs                          
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cat  /opt/linux/linux-5.4/tools/lib/api/NOTE-TRAPPED                                   
Congratulations, you found the clue!                
The next clue is in: /usr/share/emacs/26.3/etc/images/icons/allout-widgets/light-bg                         
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ ls -a /usr/share/emacs/26.3/etc/images/icons/allout-widgets/light-bg                         
.           closed.xpm         end-connector.xpm       leaf.xpm              mid-connector.xpm   skip-descender.xpm      unlocked-encrypted.xpm                                                   
..          empty.png          extender-connector.png  locked-encrypted.png  opened.png          through-descender.png           
REVELATION  empty.xpm          extender-connector.xpm  locked-encrypted.xpm  opened.xpm          through-descender.xpm                
closed.png  end-connector.png  leaf.png                mid-connector.png     skip-descender.png  unlocked-encrypted.png                          
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cd /usr/share/emacs/26.3/etc/images/icons/allout-widgets/light-bg/REVELATION                  
bash: cd: /usr/share/emacs/26.3/etc/images/icons/allout-widgets/light-bg/REVELATION: Not a directory                       
hacker@commands\~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cat /usr/share/emacs/26.3/etc/images/icons/allout-widgets/light-bg/REVELATION                          
Great sleuthing!                      
The next clue is in: /usr/share/m17n/icons                                                   

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!                      
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ ls -a /usr/share/m17n/icons                           
.                el-kbd.png           hr-kbd.png          math-latex.png     ru-kbd.png               ta-typewriter.png    vi-tcvn.png               
..               en-ispell.png        hy-kbd.png          ml-inscript.png    ru-phonetic.png          ta-vutam.png         vi-telex.png              
README-TRAPPED   eo-h-fundamente.png  ii-phonetic.png     ml-itrans.png      ru-yawerty.png           te-apple.png         vi-viqr.png         
am-sera.png      eo-h-sistemo.png     ja-anthy.png        ml-mozhi.png       sa-IAST.png              te-inscript.png      vi-vni.png              
ar-kbd.png       eo-plena.png         ja-tcode.png        ml-remington.png   sa-itrans.png            te-itrans.png        yi-yivo.png              
as-inscript.png  eo-q-sistemo.png     ka-kbd.png          ml-swanalekha.png  sd-inscript.png          te-pothana.png       zh-bopomofo.png                   
as-itrans.png    eo-x-sistemo.png     kk-arabic.png       mr-inscript.png    si-phonetic-dynamic.png  te-sarala.png        zh-cangjie.png                     
as-phonetic.png  fa-isiri.png         kk-kbd.png          my-kbd.png         si-samanala.png          th-kesmanee-2.png    zh-pinyin.png                
be-kbd.png       gu-inscript.png      km-yannis.png       ne-rom.png         si-sumihiri.png          th-kesmanee.png      zh-py-b5.png                 
bn-disha.png     gu-itrans.png        kn-inscript.png     ne-trad-ttf.png    si-transliteration.png   th-pattachote-2.png  zh-py-gb.png                
bn-inscript.png  gu-phonetic.png      kn-itrans.png       ne-trad.png        si-wijesekera.png        th-pattachote.png    zh-py.png               
bn-itrans.png    he-kbd.png           kn-kgp.png          or-inscript.png    sk-kbd.png               th-tis820-2.png      zh-quick.png                     
bn-probhat.png   hi-inscript.png      kn-optitransv2.png  or-itrans.png      sr-kbd.png               th-tis820.png        zh-tonepy-b5.png                     
bn-unijoy.png    hi-itrans.png        ko-han2.png         pa-inscript.png    sv-post.png              ua-kbd.png           zh-tonepy-gb.png                       
bo-wylie.png     hi-optitransv2.png   ko-romaja.png       pa-itrans.png      syrc-phonetic.png        unicode.png          zh-tonepy.png               
bopo-kbd.png     hi-phonetic.png      latn-post.png       pa-jhelum.png      ta-inscript.png          ur-phonetic.png      zh-zhuyin.png            
cmc-kbd.png      hi-remington.png     latn-pre.png        pa-phonetic.png    ta-itrans.png            uz-kbd.png               
cs-kbd.png       hi-typewriter.png    lo-kbd.png          ps-phonetic.png    ta-phonetic.png          vi-nom-vni.png             
dv-phonetic.png  hi-vedmata.png       lo-lrt.png          rfc1345.png        ta-tamil99.png           vi-nom.png              
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cat /usr/share/m17n/icons/README-TRAPPED                          
Great sleuthing!                 
The next clue is in: /usr/local/lib/python3.8/dist-packages/sympy/tensor                         
                        
Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!                  
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ ls -a /usr/local/lib/python3.8/dist-packages/sympy/tensor            
.  ..  SPOILER-TRAPPED  __init__.py  __pycache__  array  functions.py  index_methods.py  indexed.py  tensor.py  tests  toperators.py                  
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cat /usr/local/lib/python3.8/dist-packages/sympy/tensor/SPOILER-TRAPPED                     
Great sleuthing!                  
The next clue is in: /opt/linux/linux-5.4/arch/x86/include/generated                    
                                
The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.            
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ ls -a /opt/linux/linux-5.4/arch/x86/include/generated              
.  ..  .TRACE  asm  uapi                                       
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cd /opt/linux/linux-5.4/arch/x86/include/generated/.TRACE    
bash: cd: /opt/linux/linux-5.4/arch/x86/include/generated/.TRACE: Not a directory                 
hacker@commands~an-epic-filesystem-quest:/usr/share/doc/libwayland-cursor0$ cat /opt/linux/linux-5.4/arch/x86/include/generated/.TRACE                  
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!              
It is: pwn.college{I_iza9DbnpNi5oZNeV8OV-3heZ7.QX5IDO0wCOwMzNzEzW}                                    
                     
## Notes and Errors              
Made some silly errors like wrote cd instead of cat .                

## Reference                  
None.          
