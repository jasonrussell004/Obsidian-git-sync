```gr
car->keep;
keep->pc;
phone->drive; drive->phone;
pc->drive; drive->pc;
pc->github;
pc->local;
: [
drive:{name="Google Drive",color="black",text=""};
local:{name="Local Backup",color="black",text=""};
github:{name="GitHub Backup",color="black",text=""};
phone:{name="Phone Obsidian",color="blue",text=""};
pc:{name="PC Obsidian",color="blue",text=""};
car:{name="Android Auto",color="blue",text=""};
keep:{name="Google Keep",color="blue",text=""};
]
```

```mermaid
flowchart TD
    %% Custom Node Styling
    classDef storage fill:#1a1a1a,stroke:#555,stroke-width:2px,color:#fff;
    classDef ui fill:#0022ff,stroke:#fff,stroke-width:1px,color:#fff;

    %% ==========================================
    %% NODE DEFINITIONS
    %% ==========================================
    %% Row 1: Data Storage / Backups
    GD["Google Drive"]
    GH["GitHub Backup"]
    LB["Local Backup"]
    
    %% Row 2: User Interfaces
    PO["Phone Obsidian"]
    PC["PC Obsidian"]
    AA["Android Auto"]
    
    %% Row 3: Bottom Collector
    GK["Google Keep"]

    %% Apply Styles
    class GD,GH,LB storage;
    class PO,PC,AA,GK ui;

    %% ==========================================
    %% GRID STRUCTURE LOCKS (Invisible Alignment)
    %% ==========================================
    %% Force Row 1 Order: Left to Right
    GD ~~~ GH ~~~ LB
    
    %% Force Row 2 Order: Left to Right
    PO ~~~ PC ~~~ AA
    
    %% Force Column Alignment: Vertical Downward Drops
    GD ~~~ PO
    GH ~~~ PC
    LB ~~~ AA

    %% ==========================================
    %% ACTUAL SYSTEM LINES / ARROWS
    %% ==========================================
    %% Straight Vertical Syncs
    GD --> PO
    GH --> PC
    PC --> GK

    %% Straight Horizontal Syncs
    PC <--> GD
    PC --> LB

    %% Diagonal clean link down to bottom center
    AA --> GK

```




```
nosygraph

rootNodes: "[[PC Obsidian]]"
linkTypeFolder: "NosyGraph/LinkTypes"
rootNodeProperties: syncs_with, backups_to, sends_to
visibleLinkTypes: syncs_with, backups_to, sends_to
```

```mermaid
graph LR
    %% Node Definitions
    GD[Google Drive]:::blue
    PO[PC Obsidian]:::green
    PhO[Phone Obsidian]:::green
    GK[Google Keep]:::green
    AA[Android Auto]:::green
    GH[GitHub Backup]:::blue
    LB[Local Backup]:::blue

    %% Layout Structure & Connections
    GD <--> PO
    GD <--> PhO
    GK --> PO
    AA --> GK
    PO --> GH
    PO --> LB

    %% Styling
    classDef blue fill:#11222d,stroke:#265c63,stroke-width:2px,color:#fff;
    classDef green fill:#0d1f14,stroke:#265e31,stroke-width:2px,color:#fff;
    linkStyle default stroke:#666,stroke-width:2px;
```
