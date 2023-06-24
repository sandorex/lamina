# Lamina
Experimental linux distribution that separates the system into several parts
- The minimal base system that contains
  - Kernel and its modules
  - Bootloader
  - Drivers
  - Backup management software, restore any other system layer easily to restore whole system to default state
  - *Things that absolutely wont work in containers*
- The desktop container
  - Xorg server if needed
  - Contains the desktop environment with its configuration
  - Some essential applications/tools that should come with it
- The system container
  - Should be minimal by default
  - Preinstalled browser and terminal emulator

## Another distro?
Well it's not a distro yet, but hopefully one day\
There are few plans to make this sustainable in the long run:
- No package repositories will be made/maintained unless absolutely necessary, all the packages will come from existing distributions
- The system will focus stricly on the desktop for now, it is not meant to be used as anything else
- User friendliness is not a focus at this point in time (maybe after phase 1)
- No images will be provided at beginning of development (after phase 1)

## Plan
The plan going forward in phases

### Phase 0 (current phase)
The goal is to build a working system using desktop and system containers using minimal debian stable as the base

By building a working prototype i will see if this is possible, are there any severe limitations or issues with the approach, goals etc

<br>

<details>
<summary>Future phases</summary>

### Phase 1
- [ ] Build a script that sets up the distribution from a debian stable installation
- [ ] Make a preseed file that will install debian with packages needed for the install script to work
- [ ] Combine preseed file and the script into an ISO, maybe get someone to test things out, bare metal tests?

</details>
