# 5268 SwerveDriveTemplate

A swerve drive template based on [REVrobotics MAXSwerve Template](https://github.com/REVrobotics/MAXSwerve-Java-Template).

The goal of this template is to have some baseline functionality that will be commonly reused year to year.

# MAXSwerve Java Template v2025.1

See [the online changelog](https://github.com/REVrobotics/MAXSwerve-Java-Template/blob/main/CHANGELOG.md) for information about updates to the template that may have been released since you created your project.

## Description

A template project for an FRC swerve drivetrain that uses REV MAXSwerve Modules.

Note that this is meant to be used with a drivetrain composed of four MAXSwerve Modules, each configured with two SPARKS MAX, a NEO as the driving motor, a NEO 550 as the turning motor, and a REV Through Bore Encoder as the absolute turning encoder.

To get started, make sure you have calibrated the zero offsets for the absolute encoders in the Hardware Client using the `Absolute Encoder` tab under the associated turning SPARK MAX devices.

## Prerequisites

* SPARK MAX Firmware v25.0.0
* REVLib v2025.0.0

## Configuration

It is possible that this project will not work for your robot right out of the box. Various things like the CAN IDs, PIDF gains, chassis configuration, etc. must be determined for your own robot!

These values can be adjusted in the `Configs.java` and `Constants.java` files.

# Getting Started

Below are the steps neccessary to set up this repository and start contributing!

## Installing Locally

1. Start by [installing WPILib](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html) for your PC if you haven't already. This comes with VSCode and all the tools neccessary to build the robot code.
2. Open the "2025 WPILib VS Code" application.
3. Clone this repository which will download the code locally to your machine. There are a couple options for this step:
    * Use VS Code's command palette (ctrl+shift+p) to run the "Git: Clone" command and follow the prompts. Search for `FRC-5268-BiomechFalcons/SwerveDriveTemplate`.
    * Follow [this article](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) from GitHub to clone using all the usual ways that GitHub supports.
4. Open the folder in VS Code if you haven't already, and you are ready to start developing!

## Using a Codespace

If you are not able to download the WPILib tools or would prefer not to, this option can help you write code all in your favorite browser. Read more about codespaces [here](https://docs.github.com/en/codespaces).
