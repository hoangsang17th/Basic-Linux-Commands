# Basic Linux Commands
Các câu lệnh cơ bản trong linux giúp bạn tiết kiệm thời gian hơn cho thời gian đầu tập làm quen với hệ điều hành linux

## Các câu lệnh trong linux
1. `ls`: Liệt kê các file và thư mục trong một đường dẫn nào đó

1.1. `ls-R`: Liệt kê các tệp tin, thư mục và cả thư mục con

1.2. `ls -al`: Cung cấp thông tin chi tiết của các tệp, như hình dưới

<img src="https://www.guru99.com/images/ls-al(2).png">

1.3. `ls -a`: Liệt kê các tệp được ẩn bởi hệ thống

1.4. `pwd`: Hiển thị đường dẫn của vị trí hiện tại

1.5. `less filename`: Xem file trực tiếp trên command

1.6. `file filename`: Xác định loại dữ liệu mà tệp chứa

2. Thay đổi đường dẫn thư mục làm việc

2.1. `cd -`: Chuyển về thư mục trước nơi bạn làm việc trước đó.

2.2. `cd ..`: Di chuyển về thư mục cha

2.3. `cd ../ ../`: Di chuyển hai thư mục lên từ nơi bạn đang ở

2.4 `cd ~`: Di chuyển đến thư mục chính của người dùng từ bất cứ đâu.

3. Thao tác với tệp tin

3.1. `rm filename`: Xóa tệp tin khỏi hệ thống mà không cần xác nhận

3.2. `mv filename new_file_location`: Cho phép di chuyển tệp tin tới một địa chỉ mới

3.3. `mv filename newfilename`: Đổi tên tệp tin

4. Thao tác với thư mục

4.1. `rmdir directoryname`: Xóa một thư mục

4.2. `mv directoryname newdirectoryname`: Đổi tên thư mục

4.3. `mkdir foldername`: Tạo một thư mục mới

5. `history`: Hiển thị các câu lệnh đã nhập trong quá khứ

6. `clear`: Làm sạch màn hình ternimal của bạn

7. Thao tác với hệ thống

7.1. `sudo apt-get update`: Cập nhật tất cả các gói đã cài đặt trong hệ thống

7.2. `sudo apt-get upgrade`: Thực hiện nâng cấp phần mềm từ các gói đã cập nhập 

7.3. `sudo apt-get install packagename`: Cài đặt một gói ứng dụng

7.4. `sudo apt-get remove packagename`: Gỡ một gói ứng dụng đã cài đặt

8. `top`: Hiển thị danh sách các tiến trình đang chạy trên máy bạn

8.1. Nhấn `q` để thoát khỏi chế độ 

9. Thao tác với tệp nén

9.1. `unzip`: Giải nén

9.2. `gzip`: Nén một tệp tin hoặc thư mục với đuôi là .zip

9.4. `tar -xf archive.tar.gz`: Giải nén một tệp tin hoặc thư mục với đuôi là .tar.gz

9.5. `sudo dpkg -i package.deb`: Cài đặt gói có đuôi .deb

10. `sudo command`: Sử dụng sudo để chạy câu lệnh với đặt quyền superuser

11. `sudo apt-get update`: Cap nhap kho ung dung

## Install Important Apps

1. Cài Google Chrome - [Hoặc](https://itsfoss.com/install-chrome-ubuntu/)
> wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

> sudo dpkg -i --force-depends google-chrome-stable_current_amd64.deb

2. Cài Ibus Bamboo - [Xem thêm](https://github.com/BambooEngine/ibus-bamboo)
> sudo add-apt-repository ppa:bamboo-engine/ibus-bamboo

> sudo apt-get update 

> sudo apt-get install ibus-bamboo

> ibus restart

*Cài Ibus Bamboo trở thành phương thức nhập mặc định*

> gsettings set org.gnome.desktop.input-sources sources "[('xkb', 'us'), ('ibus', 'Bamboo')]"

Vào mục Ứng dụng → System settings → Applications → Startup → Add startup app…

Gõ lệnh sau vào mục custom command:

> ibus-daemon -drx

3. Tweaks - Tinh chỉnh hệ thống

> sudo add-apt-repository ppa:philip.scott/elementary-tweaks

> sudo apt update

> sudo apt install elementary-tweaks

> reboot

System Settings --> Tweaks --> Appearance --> Layout

> sudo add-apt-repository ppa:noobslab/macbuntu

> sudo apt-get update

> sudo apt-get install macbuntu-os-icons-v1804

> sudo apt-get install macbuntu-os-ithemes-v1804

Chọn MacBuntu-Sierra-light-soild-thin
[Xem thêm](https://www.noobslab.com/p/themes-icons.html)

4. Git - [Xem thêm](https://git-scm.com/download/linux)
> sudo apt-get install git

5. WPS Office - [Tải tại đây](https://linux.wps.com/) 
> sudo dpkg -i wps-office_11.1.0.10.161.XA_amd64.deb

6. Android Studio - [Xem thêm](https://developer.android.com/studio/install)

*Cài đặt Java JDK*

> sudo apt install openjdk-11-jdk

*Thêm kho lưu trữ android-studio*

> sudo add-apt-repository ppa:maarten-fonville/android-studio

> sudo apt update

> sudo apt install android-studio

* Cài đặt một số thư viện 32 bit cho máy 64 bit*

> sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386

7. Teamview - [Xem thêm](https://community.teamviewer.com/English/kb/articles/45-how-to-install-teamviewer-on-ubuntu)
> wget https://download.teamviewer.com/download/linux/teamviewer_amd64.deb

> sudo apt install ./teamviewer_amd64.deb

8. OBS - [Xem thêm](https://obsproject.com/wiki/install-instructions#linux)
> sudo apt install ffmpeg

> sudo add-apt-repository ppa:obsproject/obs-studio

> sudo apt update 

> sudo apt install obs-studio

9. GParted - Trình quản lý phân vùng - [Xem thêm](https://itsfoss.com/format-usb-drive-sd-card-ubuntu)
> sudo apt-get install gparted

10. GRUB Themes - [Xem thêm](https://www.gnome-look.org/browse/cat/109/order/latest/)
[Tải tại đây](https://drive.google.com/drive/folders/1Eq3jCY2Yi4aQS8ihq7RESG2AHddKrgS8?usp=sharing)

> cd 17theme

> sudo ./install.sh

11. Lampp - [Tải tại đây](https://www.apachefriends.org/xampp-files/8.0.2/xampp-linux-x64-8.0.2-0-installer.run)
> chmod 755 xampp-linux-x64-8.0.2-0-installer.run

> sudo ./xampp-linux-x64-8.0.2-0-installer.run

Khởi chạy Lampp

> sudo /opt/lampp/lampp start

Tắt Lampp
> sudo /opt/lampp/lampp stop

12. Brave Browse - [Nhanh hơn, mượt hơn](https://brave.com/)
> sudo apt install apt-transport-https curl gnupg

> curl -s https://brave-browser-apt-release.s3.brave.com/brave-core.asc | sudo apt-key --keyring /etc/apt/trusted.gpg.d/brave-browser-release.gpg add -

> echo "deb [arch=amd64] https://brave-browser-apt-release.s3.brave.com/ stable main" | sudo tee /etc/apt/sources.list.d/brave-browser-release.list

> sudo apt update

> sudo apt install brave-browser
  
## Fix Error
1. Fix add-apt-repository: command not found error
> sudo apt-get install software-properties-common

> sudo apt-get update

2. Android Studio: /dev/kvm device permission denied
> sudo apt install qemu-kvm

> sudo adduser $USER kvm

## About Author
* [Phạm Hoàng Sang](https://www.facebook.com/hoangsang17th) - VKU
* Email: phsang49@gmail.com- hoangsang17th@gmail.com
* Youtube: [Hoàng Sang SICT](https://www.youtube.com/channel/UCFovmhE6wmj-6doJKKURaiA)
* Tặng tôi một ly cafe: Ngân hàng quân đội Việt Nam - MB Bank, số tài khoảng 5050148454917
