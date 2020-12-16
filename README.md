# CouponWithoutOCP

Dalam Kodingan pada Class Coupon.cs dibawah ini, membuat class tersebut dapat menghandle diskon, persentase, dan cashback

          if(discNominal == 0 && discPercentage > 0)
          {
              net = (100 - discPercentage) * originPrice / 100;
          }
          else if (discNominal > 0 && discPercentage == 0)
          {
              net = originPrice - discNominal;
          }
          else if(discNominal > 0 && discPercentage > 0)
          {
              if(discNominal >= 3000 && discPercentage >= 30)
              {
                  net = originPrice - discNominal;
              }
              else if(discNominal < 3000 && discPercentage < 30)
              {
                  double hargadiscPersen;
                  hargadiscPersen =  (100 - discPercentage)  * originPrice/ 100;
                  net = hargadiscPersen - discNominal;
              }
          }
          return net;   
          
   ![ClassDiagramCouponWithoutOCP](https://user-images.githubusercontent.com/61864279/102340524-3a0f7500-3fc9-11eb-9493-ce9fca2ea5c3.png)

