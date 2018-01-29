NAS ([Network-attached storage](https://en.wikipedia.org/wiki/Network-attached_storage)) are really cool devices. Your personal local digital cloud which you have full control on.  

I had old device from Western Digital: WD MyBook WorldEdition II (Blue Rings version), still possible to find it on WD's legacy [site](https://support.wdc.com/product.aspx?ID=107&lang=en) or find more information about [WD MyBook](https://en.wikipedia.org/wiki/Western_Digital_My_Book#World_Edition) series on Wiki.
[![wd.jpg](https://svbtleusercontent.com/ov0umnz0ebasdg_small.jpg)](https://svbtleusercontent.com/ov0umnz0ebasdg.jpg)

WorldEdition II has 2 WD Black Series 5400 RPM hard drives, one 100/1000 Ethernet and one USB 2.0 port. Couple software RAID options are available.  

It was slow device even for 2007. Initial access was possible via MioNet site (then re-branded to WD Anywhere Access), no NFS, FTP or other technologies which come as a standard in modern NAS devices. But after I discovered [Hacking WD MyBook World Ed](http://mybookworld.wikidot.com/) it was possible to do anything with that little white box. I did not turn it to space ship but NFS access and Transmission client helped to use it in better way.  

It was working fine for years and even survived long process when we moved to United States -- and worked for 2 more years after that, but unfortunately at one day it just died. According to sound it tried to start drives spin but something was definitely wrong. I disassembled it to find couple bulgy capacitors, maybe something else was wrong too.
Then I did a big mistake -- I found closest PC repair shop, did not check any stop reviews and took it there. As it turned out 3 weeks later, they just tried to power some LEDs directly to prove that device is working, did not even take care of bad capacitors, and then tried to sell it back to me.  

The only used NAS motherboard replacement was found on Italian eBay -- while the price was ~30$, delivery cost was too high ~50$. I knew that hard drives are fine so it is a time for new NAS.  

I like cool NAS devices like [QNAP](https://www.qnap.com/en-us/) or [Synology](https://www.synology.com/en-us) produce -- it looks very sleek. But it is not the way I wanted to go. Let's build NAS from scratch.  

I already had 2x500GB drives from MyBook, and purchased two more WD Red Series 3TB drives.  

Items to do:
* get existing data from two 500GB hard drives from MyBook
* pick the rest of hardware and assembly it
* system installation -- FreeNAS, OpenMediaVault or anything else
* configure needed services -- NFS, Transmission, monitoring, whatever  

Pictures credits:
* [engadget.com](https://www.engadget.com/)
