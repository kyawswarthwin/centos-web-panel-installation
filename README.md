# CentOS Web Panel Installation
**၁) Swap File ရှိမရှိစစ်ပါ။**

    free -m
    
**၂) Swap File မရှိလျှင် အောက်ပါ Command များကိုရိုက်ပီး၊ Swap File ဆောက်ပါ။**

    sudo dd if=/dev/zero of=/swapfile count=4096 bs=1MiB
    sudo chmod 600 /swapfile
    sudo mkswap /swapfile
    sudo swapon /swapfile
    sudo echo "/swapfile swap swap sw 0 0" >> /etc/fstab
    
**၃) အောက်ပါ Link အတိုင်း CentOS Web Panel ကို Install လုပ်ပါ။**
[ဒီမှာနှိပ်ပါ](http://centos-webpanel.com/server-update)
