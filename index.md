---
layout: single
author_profile: true
title: "About Me"
permalink: /
toc: true
toc_sticky: true
toc_label: "Contents"
toc_icon: "list-ul"
---

**[日本語ページはこちら (Japanese)](/ja/)**

Hello! I am **Kurorekishi**. While I work professionally as a **Lead Programmer using Cocos Creator (TypeScript)**, my personal focus and passion lie in **Unreal Engine 5 Tool Development** and **Technical Art**.

I specialize in bridging the gap between engineering and art, developing robust editor tools and creating visually striking procedural content using **C++, UE5, HLSL, and Python**.

With a strong focus on **asset management, workflow optimization**, and **tool development**, I strive to create environments where artists can work efficiently and creativity can flourish.

## Technical Skills

**Game Engines**
![Unreal Engine 5](https://img.shields.io/badge/Unreal_Engine_5-313131?style=for-the-badge&logo=unrealengine&logoColor=white)
![Cocos Creator](https://img.shields.io/badge/Cocos_Creator-2C3E50?style=for-the-badge&logoColor=white)

**Languages**
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![HLSL](https://img.shields.io/badge/HLSL-5C2D91?style=for-the-badge&logo=directx&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Objective-C](https://img.shields.io/badge/Objective--C-3A95E3?style=for-the-badge&logo=apple&logoColor=white)

**Tools & DevOps**
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white)
![Backlog](https://img.shields.io/badge/Backlog-23AC38?style=for-the-badge&logoColor=white)

**Specialties**
* Editor Tool Development
* Procedural Material / Technical Art
* Workflow Optimization & Team Leadership

## Work Experience Highlights
- Lead Programmer - Cocos Creator / TypeScript (7 engineers, 25-person team)
- CI/CD Pipeline Implementation (Jenkins, build optimization)
- Artist/Planner Coordination & Workflow Optimization
- Junior Developer Training (2 developers, 3-month program)

## Engine Contributions

### Unreal Engine 5 Source Code
**[PR #14424: Fix missing Convert node in Material Editor context menu (Under Review)](https://github.com/EpicGames/UnrealEngine/pull/14424)**
*Note: Access to the Epic Games repository is required to view this link.*

Identified a regression bug in the Material Editor occurring in UE5.6/5.7 and submitted a C++ patch (Pull Request) to the official repository.

* **Issue:** A regression where the Convert node was excluded from search candidates when dragging from a numeric output pin and searching for "Break" or similar.
* **Root Cause Identification:** Identified that the engine's node search validation (`HasCompatibleConnection`) references static type information from the CDO (Class Default Object), whereas the new specification of `UMaterialExpressionConvert` generates pins dynamically at runtime, causing type information to be missing on the CDO and resulting in exclusion from candidates.
* **Solution:** Added logic to the C++ engine code to bypass the CDO check for the target node as a special case when the source pin is of a numeric type (`MCT_Numeric`).

## Projects

### 1. [ProceduralDrawingMaterialSamples](https://github.com/EmbarrassingMoment/ProceduralDrawingMaterialSamples)
**UE5 Sample Project / Technical Art**

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <div style="flex: 1 0 45%; min-width: 250px;">
    <img src="/assets/images/procedural/Rader.gif" alt="Radar" style="width: 100%; border-radius: 4px;">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Radar Sweep</p>
  </div>
  <div style="flex: 1 0 45%; min-width: 250px;">
    <img src="/assets/images/procedural/OldTV.gif" alt="Old TV" style="width: 100%; border-radius: 4px;">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Retro TV Effect</p>
  </div>
  <div style="flex: 1 0 45%; min-width: 250px;">
    <img src="/assets/images/procedural/PageCurl.gif" alt="Page Curl" style="width: 100%; border-radius: 4px;">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Page Curl Transition</p>
  </div>
  <div style="flex: 1 0 45%; min-width: 250px;">
    <img src="/assets/images/procedural/Snow.gif" alt="Snow" style="width: 100%; border-radius: 4px;">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Snow Crystal</p>
  </div>
</div>

A collection of textureless procedural material samples demonstrating advanced shader techniques.
*   **Key Features:** Includes diverse effects such as radar, animations, snowflakes, and transitions.
*   **Community:** Highly regarded with 145+ stars and 13+ forks on GitHub.
*   **License:** MIT License.

### 2. [MIRenamer](https://github.com/EmbarrassingMoment/MIRenamer)
**UE5 Plugin / Workflow Automation**

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <div style="flex: 1; min-width: 300px;">
    <img src="/assets/images/mirenamer/workflow.gif" alt="Batch Renaming Demo" style="width: 100%; border-radius: 4px;" loading="lazy">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Batch Renaming Demo</p>
  </div>
  <div style="flex: 1; min-width: 300px;">
    <img src="/assets/images/mirenamer/context_menu.jpg" alt="Context Menu Integration" style="width: 100%; border-radius: 4px;" loading="lazy">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Context Menu Integration</p>
  </div>
</div>

A powerful plugin for automating the naming of Material Instance assets with intelligent pattern recognition and customizable prefixes.
*   **Key Features:** Batch renaming, auto-rename on creation, command-line support (Commandlet), and multi-language UI (English/Japanese).
*   **Technical Highlights:** Context menu integration, asset registry scanning, intelligent base name extraction from multiple naming patterns, and CI/CD pipeline support.
*   **Distribution:** Available on [Fab](https://www.fab.com/listings/0523dde6-2cc5-4129-9d83-78584910d5a5).

### 3. [TextureChannelPacker (RGBPackingTool)](https://github.com/EmbarrassingMoment/RGBPackingTool)
**UE5 Plugin / Asset Optimization**

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <div style="flex: 1; min-width: 300px;">
    <img src="/assets/images/workflow.gif" alt="Workflow Demo" style="width: 100%; border-radius: 4px;" loading="lazy">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Workflow Demo</p>
  </div>
  <div style="flex: 1; min-width: 300px;">
    <img src="/assets/images/ui_overview.jpg" alt="UI Overview" style="width: 100%; border-radius: 4px;" loading="lazy">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">UI Overview</p>
  </div>
</div>

A high-performance utility for packing grayscale textures into RGBA channels, essential for optimizing game assets and creating industry-standard texture maps.
*   **Key Features:** Creates ORM/ORD maps, supports 16-bit/32-bit float textures, automatic resizing with high-quality bilinear interpolation, and multi-language UI (English/Japanese).
*   **Technical Highlights:** Multi-threaded parallel processing for fast conversion, extended format support (G8, G16, R16F, R32F, RGBA32F), cancellable progress dialog, and intelligent default handling (black for RGB, white for Alpha).
*   **Distribution:** Available on [Fab](https://www.fab.com/listings/7b231ecc-079f-45dc-9b8e-45dacc6b0771).
*   **License:** MIT License.

### 4. [QuickBaker](https://github.com/EmbarrassingMoment/QuickBaker)
**UE5 Plugin / Material Baking**

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <div style="flex: 1; min-width: 300px;">
    <img src="/assets/images/quickbaker/workflow.gif" alt="Baking Workflow" style="width: 100%; border-radius: 4px;" loading="lazy">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">Baking Workflow</p>
  </div>
  <div style="flex: 1; min-width: 300px;">
    <img src="/assets/images/quickbaker/window_en.jpg" alt="UI Overview" style="width: 100%; border-radius: 4px;" loading="lazy">
    <p style="font-size: 0.8em; text-align: center; color: #888; margin-top: 5px;">UI Overview</p>
  </div>
</div>

A lightweight editor tool designed to streamline the conversion of dynamic material expressions into static textures. It enables efficient baking of procedural noise, Signed Distance Fields (SDFs), and LUTs directly within the engine.
*   **Key Features:** Supports direct-to-asset baking (.uasset) and disk export (PNG/EXR), high-precision 16-bit float output, and workflow optimizations such as auto-naming and directory management.
*   **License:** MIT License.
*   **Distribution:** Available on [Fab](https://www.fab.com/listings/b53f5488-9b96-43cd-9963-e9fedafb56e9).

## Technical Writing

* **[UE5] Implementing a Circular Wipe Transition** - Qiita
    * A technical guide on creating a circular wipe post-process effect in Unreal Engine 5.
    * [Read on Qiita (Japanese)](https://qiita.com/EmbarrassingMoment/items/11e74b18a5488e84757d)

## GitHub Activity

<div style="display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 20px;">
  <div style="flex: 1; min-width: 300px;">
    <img src="https://github-readme-stats.vercel.app/api?username=EmbarrassingMoment&show_icons=true&theme=tokyonight" alt="GitHub Stats" style="width: 100%;" loading="lazy">
  </div>
  <div style="flex: 1; min-width: 300px;">
    <img src="https://github-readme-stats.vercel.app/api/top-langs?username=EmbarrassingMoment&layout=compact&theme=tokyonight&hide=html,css" alt="Top Languages" style="width: 100%;" loading="lazy">
  </div>
</div>

## Contact & Links

*   **GitHub:** [EmbarrassingMoment](https://github.com/EmbarrassingMoment)
*   **Twitter/X:** [@endwar1338](https://x.com/endwar1338)
*   **Fab:** [My Listings](https://www.fab.com/sellers/kurorekishi)

---
[<i class="fab fa-github"></i> View My GitHub Profile](https://github.com/EmbarrassingMoment){: .btn .btn--primary .btn--large}
