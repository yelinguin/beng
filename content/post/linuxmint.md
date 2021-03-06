---
title: "Linuxmint"
date: 2017-07-01T20:07:28+07:00
draft: false

subtitle: "กลับมาทดลองเล่น Linux Mint"
tags: ["linux", "linux mint"]
---

หลังจากได้คอมพิวเตอร์เครื่องใหม่ อยากกลับไปใช้งาน Linux
เงื่อนไข คือ ต้องเล่น Steam ได้ เพราะจะเอามาตีดอท ฮ่าๆ และที่สำคัญต้องมีไดรเวอร์การ์ดไวเลสที่ซื้อมาแบบพร้อมใช้งาน (ขี้เกียจ)
จากประสบการณ์ควรใช้ชิปของ Intel (Broadcom ต้องออกแรงอีก เหนื่อย)

ให้ง่ายต้องเลือก Ubuntu Derivative เลือก Mint (ลีนุกซ์เลขไทย 2 แปลกดี) เคยเล่นแล้วประทับใจดี เลือกใช้เวอร์ชั่น Cinnamon 18.1 Serena ซึ่งพัฒนาจาก Ubuntu 16.04

จากนั้น จึงดาวน์โหลดไฟล์ ISO แล้วมายัดใส่ USB เนื่องจากไม่มีสายไฟ Molex to SATA (Power Supply มีไม่พอ เห้อ แต่ขน DVD-ROM มาจากบ้านเลยนะนั่น)
โดยใช้โอเพ่นซอร์สตัวนึงชื่อ [Rufus](https://rufus.akeo.ie/ "Rufus; Create bootable USB drives the easy way") เป็นอันเสร็จเรียบร้อย


ทดลองเล่นจาก USB แบบยังไม่ได้ติดตั้ง ใช้งานได้ดี (ไวเลสก็เห็น โอเคเลย อย่างอื่นค่อยว่ากัน) หลังจากติดตั้ง

- ตรวจสอบฮาร์ดแวร์ว่าใช้งานได้ปกติดีไหม

- ติดตั้งโปรแกรมใช้งานต่างๆ เช่น System Monitor ต่างๆ

- ติดตั้งไดรเวอร์การ์ดจอ เนื่องจากผมใช้งานออนบอร์ด ซื้อ Intel G4560 มาใช้ ได้ Intel HD Graphics 610 โหลดมาติดตั้งจาก [1.org ](https://01.org/linuxgraphics "Intel Graphics for Linux") (ชื่อเว็บเท่ห์สัด)

- ติดตั้งไดรเวอร์เมาส์ SteelSeries Rival 100

และพบปัญหาใหญ่ คือ **ปิดเครื่องแล้วไม่ดับ (งานเข้าเลย)** ทดลองแก้ โดยหาข้อมูลจากเว็บไซต์

- แก้ไฟล์ mdm config (/usr/share/mdm/default) ไปเปลี่ยนออพชั่น shutdown -P แทน **(ไม่หาย)**

- เปลี่ยน Display Manager or Login Managerเป็นตัวอื่น (Default คือ MDM) ผมเลือก GDM (Gnome นั่นเอง) ปรากฏว่าหายเป็นปลิดทิ้ง ตอนแรกโง่ตั้งนาน หาวิธีเปลี่ยนไปใช้งานไม่เจอ (สามารถเลือกกดตอนหน้าล็อกอิน)

- หลังจากเปลี่ยนตอนแรกเหมือนจะต้องลบ MDM ทิ้งไปเลย ทำให้เข้าใช้งานหน้า Gnome Shell (ต้องเข้าโดย startx ไม่รู้สาเหตุอะไร) ซึ่งผมไม่ชอบอย่างแรง (UX ไม่ใช่สไตล์ผมมั้ง เอออะ จะให้เสิร์ชอย่างเดียว บ้าป่าว) พอเลือกเข้า Cinnamon เหมือนเดิมได้ก็โอเคเลย

- จะลองไปติตดั้ง Ubuntu Gnome แล้ว แต่แก้ปัญหาได้ก่อน

</br></br>
ขอจบเรื่องไว้เพียงเท่านี้ สวัสดี

โกโรโกโส
