# Contributing to Inky

First off, thank you for considering contributing to Inky!
Building a portable console is a massive undertaking, and we welcome help across hardware design, operating system development, and game engine tooling

## 1. Finding Something to Do

Before you start working, make sure your efforts align with the project's current goals

  Check our central GitHub Project Board to see what is currently in progress
  Look for issues that are assigned to no one
  If you have a new idea, please open an issue first to discuss it before writing code or designing hardware

## 2. General Workflow

We use a standard fork-and-pull-request workflow
  Fork the relevant repository (hw-shell, sw-launcher, etc.)
  Branch out from the main branch. Name your branch descriptively (e.g., feature/wifi or hardware/dpad)
  Commit your changes clearly
  Push to your fork and open a Pull Request (PR) against our main branch

## 3. Software Guidelines

  Ensure your code builds successfully on the target hardware (or emulator, if applicable) before submitting
  Do not submit massive PRs that change thousands of lines. Break large changes into smaller, reviewable chunks
  Remove all debug print statements before opening your Pull Request

## 4. Hardware & Design Guidelines

Working with physical design files requires a slightly different approach, as GitHub cannot easily highlight the differences between two 3D models or PCB files

  CAD Files: Always include exported .STEP files alongside your native project files (e.g., Fusion360, FreeCAD) so anyone can review the geometry
  PCBs: If submitting a PCB change, export and include the updated Gerbers in your PR
  Visual Proof: Because binary hardware files cannot be diffed, you must include screenshots in your Pull Request description showing exactly what changed visually
  Printability: If you modify the shell, ensure the new geometry can actually be manufactured (e.g., avoiding impossible overhangs for 3D printing or injection molding)
