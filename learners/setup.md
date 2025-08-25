---
title: Setup
---

# Setup

## Logging into Rivanna/Afton

To log into the Rivanna or Afton HPC cluster, start by visiting the **HPC Login Instructions** page:  
[https://www.rc.virginia.edu/userinfo/hpc/login/](https://www.rc.virginia.edu/userinfo/hpc/login/)

Follow the instructions for **Secure Shell Access (SSH)** based on your operating system:  

- **Windows**: Install the recommended SSH client, **MobaXterm**, by clicking the *Install MobaXterm* button under the Windows section of the page and following the instructions.  
- **macOS**: Open the **Terminal** application, located in the *Utilities* folder.  
  - On macOS Mojave and earlier, the default shell is **Bash**.  
  - On macOS Catalina and later, the default shell is **Zsh**. To temporarily switch to Bash, open Terminal, type `bash`, and press <kbd>Return</kbd>.  
- **Linux**: Most Linux systems use **Bash** as the default shell. Open a terminal using the Applications menu or search bar (look for **Terminal**, **Konsole**, or **xterm**). If your system defaults to another shell, you can switch by typing `bash` and pressing <kbd>Return</kbd>.  

Once you have a terminal open, connect to the HPC cluster by typing:

```bash
ssh -Y uva_compute_id@login.hpc.virginia.edu
```

Replace `uva_compute_id` with your UVA computing ID. You will then be prompted to enter your UVA NetBadge password.

## Data Access for This Lesson
Before we start, let’s make sure you are in your home directory. In the terminal, type:

```bash
cd
```

and press <kbd>Return</kbd>.

The data for this lesson is stored in the folder:

```bash
/standard/bims6000/shell-lesson-data
```

Let’s copy this folder into your home directory so you can work with your own copy. Run the following command:

```bash
cp -r /standard/bims6000/shell-lesson-data .
```

Don’t worry about the details of this command yet. We will explain how it works later in the lesson.

