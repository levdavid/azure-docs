---
 title: include file
 description: include file
 services: bastion
 author: cherylmc
 ms.service: bastion
 ms.topic: include
 ms.date: 06/02/2022
 ms.author: cherylmc
 ms.custom: include file
---

1. In the [Azure portal](https://portal.azure.com), go to the virtual machine that you want to connect to. On the **Overview** page, select **Connect**, then select **Bastion** from the dropdown.

   :::image type="content" source="./media/bastion-vm-rdp/connect.png" alt-text="Screenshot of Connect." lightbox="./media/bastion-vm-rdp/connect.png":::

1. After you select Bastion from the dropdown, a side bar appears that has three tabs: RDP, SSH, and Bastion. Because Bastion was provisioned for the virtual network, the Bastion tab is active by default. Select **Use Bastion**.

   :::image type="content" source="./media/bastion-vm-rdp/select-use-bastion.png" alt-text="Screenshot of Select Use Bastion.":::

1. On the **Connect using Azure Bastion** page, enter the username and password for your virtual machine. If your VM is domain-joined, you must use the following format: **username@domain.com**. Then, select **Connect**. 

   :::image type="content" source="./media/bastion-vm-rdp/connect-vm-host.png" alt-text="Screenshot of Connect button.":::

1. The RDP connection to this virtual machine via Bastion will open directly in the Azure portal (over HTML5) using port 443 and the Bastion service. 

   * When you connect, the desktop of the VM may look different than the example screenshot. 
   * Using keyboard shortcut keys while connected to a VM may not result in the same behavior as shortcut keys on a local computer. For example, when connected to a Windows VM from a Windows client, CTRL+ALT+END is the keyboard shortcut for CTRL+ALT+Delete on a local computer. To do this from a Mac while connected to a Windows VM, the keyboard shortcut is Fn+CTRL+ALT+Backspace.

   :::image type="content" source="./media/bastion-vm-rdp/connection.png" alt-text="Screenshot of Connect using port 443.":::
