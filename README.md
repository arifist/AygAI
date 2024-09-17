# AygAI

*Projeyi Airlines.py dosyasından çalıştırabilirsiniz.
*Gözetimli öğrenme kısa sürede çalışarak yüksek performans sonuç üretiyor.
* 103 bin veri olduğundan Gözetimsiz öğrenme için ise program 30 dk gibi bir süre sonra sonuçlanıyor.
*Ayrıca bir flask api yazarak kullanıcların kriterlere verdiği puanları hesaplayıp kullanıcıların genel memnuniyetini tahmin eden bir web arayüzü tasarladım. buna ulaşmak içinde app.py uygulamasını çalıştırıp localhost:8080 portuyla çalıştırılabilir.
*Resim dosyalarımda ise programın ürettiği grafik çıktıları bulunmaktadır.

Sonuçlar:
*Gözetimli Öğrenim(RandomForestRegressor):
Özelliklerin Genel Memnuniyet Puanına Katkısı:
Inflight_wifi_service: 0.210610675609222
Departure/Arrival_time_convenient: 0.040966447184388015
Ease_of_Online_booking: 0.0215439760929084
Gate_location: 0.0358979681268821
Food_and_drink: 0.04100122745059538
Online_boarding: 0.3508358165484226
Seat_comfort: 0.02430713992829045
Inflight_entertainment: 0.07811207667400526
On-board_service: 0.03035791962411771
Leg_room_service: 0.05410116241614094
Baggage_handling: 0.02531509463427212
Checkin_service: 0.030614399264681107
Inflight_service: 0.027864995566146696
Cleanliness: 0.028471100879927144

Doğruluk: 94.64%

*Gözetimsiz Öğrenim(K-Means):
Küme Merkezleri:
   Inflight_wifi_service  Departure/Arrival_time_convenient  \
0               3.082696                           3.173233   
1               2.284870                           2.917452   

   Ease_of_Online_booking  Gate_location  Food_and_drink  Online_boarding  \
0                2.966676       3.007184        3.854880         3.767510   
1                2.492668       2.939011        2.379331         2.598804   

   Seat_comfort  Inflight_entertainment  On-board_service  Leg_room_service  \
0      4.159696                4.265727          3.882768          3.745802   
1      2.532295                2.214585          2.752160          2.854259   

   Baggage_handling  Checkin_service  Inflight_service  Cleanliness  
0          4.053994         3.618599          4.068639     4.038812  
1          3.099372         2.908178          3.101423     2.337981  
