# penjumlahan-dalam-JS-didalam-PHP
Penjumlahan JS didalam PHP

          <?php 
                  $script = <<< JS
                  $('input#tpreorder-tpreorderrefmulti-0-harga.form-control, input#tpreorder-tpreorderrefmulti-0-jumlah.form-control').keyup(function(){
                      var jmlId = $('input#tpreorder-tpreorderrefmulti-0-jumlah.form-control').val();
                      var harga = $('input#tpreorder-tpreorderrefmulti-0-harga.form-control').val();
                      var hasil = Number(harga)* Number(jmlId);
                      if ( jmlId != "" && harga != "" ) {
                          $('input#tpreorder-tpreorderrefmulti-0-harga2.form-control').val(hasil);
                          }
                      });
                  JS;
                  $this->registerJs($script);
              ?>
