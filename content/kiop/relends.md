---
title : "Relends"
summary : "relend"
---
{{< border >}}
_009.cpp_
{{< /border >}}

```
#LQFOXGH <FDUO.K>
XVLQJ QDPHVSDFH VWG;
 


LQW PDA(LQW D, LQW E) { UHWXUQ (D > E) ? D : E; }
 


LQW NQDSVDFN(LQW Z, LQW ZW[], LQW YDO[], LQW Q)
{
 
 
    LI (Q == 0 || Z == 0)
        UHWXUQ 0;
 

    LI (ZW[Q - 1] > Z)
        UHWXUQ NQDSVDFN(Z, ZW, YDO, Q - 1);
 
    HOVH
        UHWXUQ PDA(
            YDO[Q - 1]
                + NQDSVDFN(Z - ZW[Q - 1], ZW, YDO, Q - 1),
            NQDSVDFN(Z, ZW, YDO, Q - 1));
}
 

LQW PDLQ()
{
    LQW YDO[] = { 60, 100, 120 };
    LQW ZW[] = { 10, 20, 30 };
    LQW Z = 50;
    LQW Q = VLCHRI(YDO) / VLCHRI(YDO[0]);
    FRXW << NQDSVDFN(Z, ZW, YDO, Q);
    UHWXUQ 0;
}
```

[Hmmmmmm]({{< ref "/tocarl" >}} "hey carlie")