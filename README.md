# Contacts:
In case of any bug or suggestion, please contact # cheetahcointools@gmail.com

# CheetahcoinMultiWalletManager
First Multi Wallet Manager for Cheetahcoin-qt/Cheetahcoind

For more information about Cheetahcoin, please visit: https://cheetahcoin.org/

# Contextualization: 
Cheetahcoin runs on a decentralized blockchain and it is much more profitable if each miner runs on a different wallet, since only Android phones can mine at difficulty "12". 
In some rare cases, computer CPUs can reach this low difficulty, cheetahcoin miner works in parallel with the cheetahcoin wallet, this means the miner will use the wallet and start the function setgenerate true <threads>.

The first Question I imagine appearing right now is:
"Why should I run the miner then if I have the wallet and can run that function myself on the wallet console?"

To be honest, there's a reason, most of the time, the android phones will not be able to find any blocks due to the network competition, it would be really hard for an android phone to find a block at such high difficulty as 2M or even 13M as per recorded as max difficulty until today. 

Having an Android machine mining in such circumstances would lead to overheating of the machine and that's dangerous on any hardware that has no cooling system.

In order to avoid this problem, cheetahcoin miner checks when the network difficulty is low enough for your to start mining and finding blocks, avoiding issues with your phone's battery or with any other component, increasing your profits, and avoiding the need of buying any new phone/tablet/pc due to mining.

Unfortunately, in order to verify the hashrate, the balance, and immature balance, actual block, or any other info of each device/wallet, you have to physically access them or access them by ssh. This may not seem to be a problem to someone who has 1/2 machines connected and mining 24/7. 
Let's put my situation up, on my side I may count on 1 Windows, 2 raspberry pi 4, 1 raspberry pi 3, and 6 Android phones. 

As you may imagine, this is not easy to manage every day, there was a moment where I would only check the devices once per day, this means that if they shut down 5 minutes after I've turned them on I would only know almost 24 hours later. 
This is not profitable, I was having my phones connected 24/7 doing nothing? 
- Unacceptable!

This project will ensure the easy management of all your cheetahcoin rigs/wallets using any phone or device on your local network.

Requirements:
  
    [windows]
      - xampp
  
    [debian/ubuntu]
      - apache2
      - phpmyadmin
      - php
      - mysql-server
  
Setup:
  
    [windows]
      Download all the project files from last release and move them to c:\xampp\htdocs\
      Execute xampp and start Apache and MySQL
      Go to c:\xampp\htdocs\managerdb and upload the project database into phpmyadmin ( http://127.0.0.1/phpmyadmin )
      Change database host,username,password and database on the file c:\xampp\htdocs\phpIncludes\connection.php
      Once done go to http://127.0.0.1/ to access your dashboard [default username:password => chtamaster:chtamaster]

    [debian/ubuntu]
      Download all the project files from last release and move them to /var/www/html/
      Start apache2 and mysql-server service 
      Go to /var/www/html/managerdb and upload the project database into phpmyadmin ( http://127.0.0.1/phpmyadmin )
      Change database host,username,password and database on the file /var/www/html/phpIncludes/connection.php
      Once done go to http://127.0.0.1/ to access your dashboard [default username:password => chtamaster:chtamaster]
  
In case of doubts please send an e-mail to:  cheetahcointools@gmail.com
  
In order to get priority in response speed follow the rules below:
  
  
       Priority  | Subject
  
       (1)       | CCMWMWR - Windows Issue/Vulnerability Report
  
       (1)       | CCMWMLR - Linux Issue/Vulnerability Report
  
       (2)       | CCMWMWI - Windows Installation & Configuration Help
  
       (2)       | CCMWMLI - Linux Installation & Configuration Help
  
       (3)       | CCMWMWS - Windows Support
  
       (3)       | CCMWMLS - Linux Support
