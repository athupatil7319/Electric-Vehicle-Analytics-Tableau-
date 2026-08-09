# Calculated Fields

## Total Electric Vehicles
## Total Manufacturers
## Total BEV Vehicles
## Total PHEV Vehicles
## BEV Percentage
```tableau
COUNTD([DOL Vehicle ID])

COUNTD([Make])

COUNTD(
    IF [Electric Vehicle Type] =
    "Battery Electric Vehicle (BEV)"
    THEN [DOL Vehicle ID]
    END
)

COUNTD(
    IF [Electric Vehicle Type] =
    "Plug-in Hybrid Electric Vehicle (PHEV)"
    THEN [DOL Vehicle ID]
    END
)

[Total BEV Vehicle] / [Total Electrical Vehicles]
