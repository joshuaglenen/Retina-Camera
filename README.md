# Introduction

This project explores the design of a low-cost, modular fundus camera for retinal imaging. Using off-the-shelf optics and a machine-vision camera, it demonstrates that high-quality fundus imaging can be achieved at a fraction of the cost of existing commercial systems.

## Purpose

Allows a physician to observe fundus images including the retina, macula, optic disc, and blood vessels. Can be used to observe signs of glaucoma, diabetic retinopathy, macular degeneration, retinal tears, intraocular tumors, etc.

## Design

    Optics: Swappable 20D lens, beam splitter, polarizer cartridges, diffuser, NIR/white LED coaxial illumination.

    Electronics: Custom STM32-based motherboard with LED drivers, buck converters, and GPIO interface to a Blackfly S camera. Powered via external 12 V DC supply.

    Enclosure: Fully modeled in Fusion 360 with integrated lamphouse, eyecup, tripod mount, and modular filter holders.

    Modularity: PCB designed in KiCad with separable functions (power, LED drivers, MCU control) for easy modification or replacement.

<img width="1520" height="722" alt="FUNDUS_CAMERA" src="https://github.com/user-attachments/assets/e5c0e74d-55de-46f3-9412-7e8f2a66fe51" />


Fig 1: Camera Modules


<img width="1520" height="722" alt="FUNDUS_CAMERA_2" src="https://github.com/user-attachments/assets/ad0d6227-f1a5-448e-af5c-06d3cbac0321" />


Fig 2: Camera Assembled


<img width="1724" height="930" alt="FundusCamMotherboard" src="https://github.com/user-attachments/assets/078f4eb0-adfe-4159-a091-463a6eeb0a18" />


Fig 3: Motherboard


## Components

    STM32F446 MCU

    TPS62133 buck regulator

    AL8860 constant-current driver (NIR LEDs)

    LM3644 dual LED flash driver (white LEDs)

    FLIR Blackfly S industrial camera

    20D ophthalmic lens

    Polarizing filters

    Optional colour filter

    LED light diffuser

    Beam splitter

    Modular eyecup


## Results

While the prototype has not been fabricated, CAD modeling and optical layout demonstrate feasibility. Comparable systems retail for $5,000–$10,000+, suggesting strong potential for a cost-reduced alternative. Future work would validate illumination levels, thermal performance, and manufacturability.
