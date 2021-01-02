---
title: "Specialized Levo Battery (gen2) Upgrades"
categories:
  - Blog
  - MTB
  - DIY
tags:
  - Post Formats
  - readability
  - standard
---

Introduced in late 2018, but sold as the 2019 Specilized Levo, the 2nd generation Levo made significant upgrades over the prior version. With the change, Specialized made major changes to the batteries. The prior (gen1) versions incorporated a lot of the 'brains' into the battery itself. This changed in the gen2 models, as the main 'brain' moved into a module built into the frame. This changed helped simplify the batteries themselves. 

The batteries now mostly only consist of the cells (18650 or 21700), a BMS (Battery Management System), and the RoPD® chrager/power connector (Rosenberger Power Data). This is what lead me to investigate what it would take to upgrade the battery packs themselves. Specifically, upgrade the base 500Wh battery to the, at the time unavailable 700Wh batteries.

So, what does the inside of the battery pack look like?
![Inside Levo Battery 01](/assets/specialized_levo/battery_inside_01.jpg)
![Six cell modules](/assets/specialized_levo/battery_six_cell.jpg)

The battery itself is a 36v (nominal) pack, which consists of 40 individual cells. They're configured in a 10s4p layout, which means ten cells in series which make up a 36v pack, each cell being 3.6v, and four of those are connected in parallel to increase the capacity. But the pack itself isn't laid out as straight forward as one would think, based on the 10 x 4 configuration. To fit the pack's layout, the cells are arranged in six-cell groupings, with six of those, and a single four cell group. 

The basic 500Wh pack is made up of 40 [Samsung INR18650-35E cells](https://www.orbtronic.com/content/samsung-35e-datasheet-inr18650-35e.pdf). At my initial time of discovery, I didn't have access to the 700Wh battery. But knew that 18560 cells basically top out at 3500mAh capacity, based on chemistry limits. The cells used here are rated at 3350mAh, which puts the actual calculated capacity at 482Wh, which they round up to 500Wh, or they use 37v as the nominal (when it's only 36v by standard calculation).

Side note: If you ever see someone advertising an 18650 cell with more than 3500mAh capacity, it's a lie. The cells in this pack are rated at 3350mAh capacity. It was my plan to figure out a way to incrase the capacity to the known existing 700Wh. In order to do this, we'd need to get up 5000mAh per cell. Luckily, the main battery enclosure has extra space in it, so we can increase the cell size. Introduce the 21700 cells. These are sometimes referred to as simply 2170 or Tesla Cells, as they're the cells used to make up the battery packs in all of the Tesla vehicles (prior to 2021). I found some sellers of new 21700 cells INR21700. With a capacity of 5000mAh, this would allow for a pack of 720Wh. So this is the route I took.

![18650 Cell](/assets/specialized_levo/battery_18650_cell.jpg)
![21700 Cell](/assets/specialized_levo/battery_21700_cell.jpg)
![Cell comparison](/assets/specialized_levo/battery_18650_21700.jpg)

With the extra space provided in the battery housing, I opted to utilize 3D Printing to make new cell holders, and create new cell internals.
![Cell modules early prototype](/assets/specialized_levo/battery_modules.jpg)
![3D Print Cell Holder 01](/assets/specialized_levo/battery_holder_6_a.jpg)
![3D Print Cell Holder 02](/assets/specialized_levo/battery_holder_4_a.jpg)

I've created a two full modules now, and simply need to put it through it's paces.