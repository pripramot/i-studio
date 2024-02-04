# i-studio
This repository is a special gift for my Thai friend. It was built using hashnode clone


การติดตั้ง
หากคุณไม่ได้ใช้สคริปต์สแตนด์อโลนหรือ@pnpm/exeติดตั้ง pnpm คุณจะต้องมี Node.js (อย่างน้อย v16.14) เพื่อติดตั้งบนระบบของคุณ

การใช้ 
คุณสามารถติดตั้ง pnpm ได้แม้ว่าคุณจะไม่ได้ติดตั้ง Node.js โดยใช้สคริปต์ต่อไปนี้

บน 
การใช้ PowerShell:

iwr https://get.pnpm.io/install.ps1 -useb | iex

บน 
curl -fsSL https://get.pnpm.io/install.sh | sh -

หากคุณไม่ได้ติดตั้ง curl คุณต้องการใช้ wget:

wget -qO- https://get.pnpm.io/install.sh | sh -

บนอัลไพน์ 
# bash
wget -qO- https://get.pnpm.io/install.sh | ENV="$HOME/.bashrc" SHELL="$(which bash)" bash -
# sh
wget -qO- https://get.pnpm.io/install.sh | ENV="$HOME/.shrc" SHELL="$(which sh)" sh -
# dash
wget -qO- https://get.pnpm.io/install.sh | ENV="$HOME/.dashrc" SHELL="$(which dash)" dash -

การติดตั้ง 
ก่อนที่จะรันสคริปต์การติดตั้ง คุณสามารถเลือกตั้งค่าตัวแปร env PNPM_VERSIONเพื่อติดตั้ง pnpm เวอร์ชันเฉพาะได้:

curl -fsSL https://get.pnpm.io/install.sh | env PNPM_VERSION=<version> sh -

เคล็ดลับ
คุณสามารถใช้ คำสั่ง pnpm envเพื่อติดตั้ง Node.js

การใช้งาน 
ตั้งแต่เวอร์ชัน 16.13 เป็นต้นมา Node.js ได้จัดส่งCorepackสำหรับการจัดการผู้จัดการแพ็คเกจ นี่เป็นคุณลักษณะทดลอง ดังนั้นคุณต้องเปิดใช้งานโดยเรียกใช้:

ข้อมูล
หากคุณได้ติดตั้ง Node.js ด้วยpnpm envCorepack จะไม่ถูกติดตั้งบนระบบของคุณ คุณจะต้องติดตั้งแยกต่างหาก ดู#4029 .

corepack enable pnpm

หากคุณติดตั้ง Node.js โดยใช้ Homebrew คุณจะต้องติดตั้ง corepack แยกต่างหาก:

brew install corepack

สิ่งนี้จะติดตั้ง pnpm บนระบบของคุณโดยอัตโนมัติ

คุณสามารถปักหมุดเวอร์ชันของ pnpm ที่ใช้ในโปรเจ็กต์ของคุณได้โดยใช้คำสั่งต่อไปนี้:

corepack use pnpm@latest

สิ่งนี้จะเพิ่ม"packageManager"ฟิลด์ในเครื่องของคุณpackage.jsonซึ่งจะสั่งให้ Corepack ใช้เวอร์ชันเฉพาะในโปรเจ็กต์นั้นเสมอ สิ่งนี้มีประโยชน์หากคุณต้องการความสามารถในการทำซ้ำ เนื่องจากนักพัฒนาทั้งหมดที่ใช้ Corepack จะใช้เวอร์ชันเดียวกันกับคุณ เมื่อมีการเผยแพร่ pnpm เวอร์ชันใหม่ คุณสามารถรันคำสั่งด้านบนอีกครั้งได้

การใช้ 
เรามีแพ็คเกจ pnpm CLI สองแพ็คเกจpnpmและ@pnpm/exe.

pnpmเป็น pnpm เวอร์ชันธรรมดาซึ่งต้องใช้ Node.js จึงจะทำงาน
@pnpm/exeถูกรวมแพ็กเกจด้วย Node.js ไว้ในไฟล์ปฏิบัติการ ดังนั้นจึงอาจใช้กับระบบที่ไม่ได้ติดตั้ง Node.js ได้
npm install -g pnpm

หรือ

npm install -g @pnpm/exe

การใช้ 
หากคุณติดตั้งตัวจัดการแพ็กเกจไว้ คุณสามารถติดตั้ง pnpm ได้โดยใช้คำสั่งต่อไปนี้:

brew install pnpm

การใช้ 
หากคุณติดตั้ง winget คุณสามารถติดตั้ง pnpm ได้โดยใช้คำสั่งต่อไปนี้:

winget install pnpm

การใช้ 
หากคุณติดตั้ง Scoop คุณสามารถติดตั้ง pnpm ได้โดยใช้คำสั่งต่อไปนี้:

scoop install nodejs-lts pnpm

การใช้ 
หากคุณติดตั้ง Chocolatey คุณสามารถติดตั้ง pnpm โดยใช้คำสั่งต่อไปนี้:

choco install pnpm

การใช้ 
หากคุณติดตั้ง Volta คุณสามารถติดตั้ง pnpm ได้โดยใช้คำสั่งต่อไปนี้:

volta install pnpm

เคล็ดลับ
คุณต้องการใช้ pnpm บนเซิร์ฟเวอร์ CI หรือไม่? ดู: การบูรณาการอย่างต่อเนื่อง




<p align="center">
  <a href="https://i-studio-steel.vercel.app">
    <img src="/public/WhatsApp Image.png" alt="WhatsApp Image" />
  </a>




