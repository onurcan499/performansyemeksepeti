# performansyemeksepeti
Food order application on C#
          if ( textBox2.Text == "")//eğer kullanıcı adı veya şifre boşsa;
            {
                MessageBox.Show("Kullanıcı adı ve/veya şifre boş geçilemez");
                hak --;
            }         
            else
            {
                if (textBox1.Text =="onurcan"&& textBox2.Text=="1234" ||textBox1.Text =="yunusemreuzun"&& textBox2.Text=="5678")
                    //kullanıcı adı ve şifre doğruysa;
                {
                    Form2 yeni = new Form2();
                    yeni.Show();
                    this.Hide();
                }
                 else 
                {
                    //hatalı şifre veya kullanıcı adı;
                    MessageBox.Show("hatalı şifre veya kullanıcı adı" );
                    hak--;
                    if(hak == 0)//hak biterse programın kapanması
                    {
                        this.Close();
                    }
            ---------------
            }
                if (textBox1.Text == "onurcan")//kayıtlı iki kişinin kullanıcı adı verilirse;
            {
                label2.Text = ("Şifreniz: 1234");
            }
            else if (textBox1.Text == "yunusemreuzun")
            {
                label2.Text = ("Şifreniz: 5678");
            }
            else
            {
                //verilmezse;
                MessageBox.Show("kullanıcı bulunamadı");
                hak--;
                if (hak == 0)
                {
                    this.Close();                       
                }
            }
            -------------------
                 sayac++;
            if (sayac == 3)
            {
                button1.Enabled =false;//  sipariş edilemez
                label1.Text = ("Bu Yemeği üretilenden fazla sipariş ettiniz");
               
            }
            
            if (sayac == 1)
            {
                label1.Text = ("1.Burger Sipariş Edildi");
                button1.Enabled = true;
                button3.Enabled = true;
            }
            if (sayac == 2)
            {
                label1.Text = ("2.Burger Sipariş Edildi");
                button1.Enabled = true;
                button3.Enabled = true;

            }
            if (sayac == 0)
            {
             
                button1.Enabled = true;
                button3.Visible = false ; // sipariş 0 olursa iptal edilemez

            }
            button3.Visible = true;//button3'ün görünürlüğünün açılması
            -----
                   if (sayac == 0)
            {
                button1.Enabled = true;
                label1.Text = ("");
                button3.Visible = false;

            }
            if (sayac == 1)
            {
                label1.Text = ("1.Burger Sipariş Edildi");
                button1.Enabled = true;
                button3.Enabled = true;
               
            }
            if (sayac == 2)
            {
                label1.Text = ("2.Burger Sipariş Edildi");
                button1.Enabled = true;
                button3.Enabled = true;
                
            }
            if (sayac == 3)
            {
                button1.Enabled = false;
                button3.Enabled = true;
               
            }
                   
        }
            }   
            
            
        }
