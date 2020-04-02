# uspay



Пример работы с классом:

``````
<?php
		require ('uspayClass.php');
 $token = '48114a98f92e'; /// Токен API выводов
 $to = '347286423473246'; ///Яндекс кошелек на который производится выводов
 $amount = 10; /// Сумма вывода
        $uspay = new UspayApi($token);
      $payment =  $uspay -> moneyback(
            [
                'amount' => $amount,
                'to'=>$to,
                ]
            );
	    ?>
``````
