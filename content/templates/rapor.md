<%*
const today = tp.date.now("YY-MM-DD")
await tp.file.rename("Rapor " + today)
%>
YKS'ye: <%*
const yks = new Date("2026-06-20")
const today_2 = new Date()
const diff = Math.ceil((yks - today_2) / (1000*60*60*24))
tR += diff + " gün"
%>

## Toplam Saat: 


## Yaptıklarım


## Notlar
