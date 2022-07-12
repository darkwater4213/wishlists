# Dynamic Loadouts (A Mock-up)  

"meta" describes what the file is, what it does, etc.
Could be: type: loadouts, uh.... idk what else DIM stores tbh
kind describes what sort of whatever it is it is. So, dynamic is a KIND of loadout. Other options under loadout would be: static (classic laodouts), hybrid (some items are static, some items aren't).
sub further describes what it is. share means that when you open it (through the share link), it's copied to your list of loadouts and is editable. ruleset means that it's NOT editable (except by the owner), an editable copy is put in your list if you so desire (with a simple yes/no dialogue), and whether or not your character meets the ruleset is displayed to your fireteam in DIM[1]. Obviously, only the actual "do i meet the ruleset" would be sent (idk what bungie's policies are on sharing character's info, tho there is the "inspect" thing in d2)

```json
{
    "meta": {
        "type": "loadout",
        "kind": "dynamic",
        "sub": "ruleset",
        "name": "Private Match 7/9/2022",
        "notes": ""
    },
    "char": {
        "class": "global",
        "subclass": {
            "rule": "-is:stasis",
            "super": "",
            "class": "",
            "jump": "",
            "melee": "",
            "grenade": "",
            "aspects": ["", ""],
            "fragments": ["", "", "", "", "", ""],
            "tree": ""
        },
    },
    "weapons": {
        "rule": "-is:exotic power:<=1560",
        "kinetic": {
            "rule": "-is:stasis",
            "mod": "",
            "shader": "",
        },
        "energy": {
            "rule": "",
            "mod": "",
            "shader": "",
        },
        "power": {
            "rule": "-is:stasis -is:linearfusionrifle",
            "mod": "",
            "shader": "",
        },
        "globalmod": "-\"full auto retrofit\"",
        "globalshader": ""
    },
    "armor": {
        "rule": "-is:exotic",
        "head": "",
        "arms": "",
        "chest": "",
        "legs": "",
        "class": ""
    },
    "fashion": {
        "rule": "",
        "shaders": {
            "head": "",
            "arms": "",
            "chest": "",
            "legs": "",
            "class": ""
        },
        "ornaments": {
            "head": "",
            "arms": "",
            "chest": "",
            "legs": "",
            "class": ""
        }
    }
    "general": {
        "ghost": {
            "rule": "-\"kill-tracker ghost\"",
            "mods": ["", "", "", ""],
            "shader": "",
            "projection": ""
        },
        "vehicle": {
            "rule": "",
            "shader": "",
        },
        "ship": {
            "rule": "",
            "shader": "",
            "transmat": ""
        },
        "emblem": {
            "rule": "",
            "tracker": ""
        }
    },
    "mods": {
        "rule": "",
        "head": {
            "rule": "",
            "general": "",
            "item": ["", ""],
            "raid": {
                "vog": "",
                "lastwish": "",
                "gos": "",
                "dsc": "",
                "votd": "",
                /* etc; idk all the raids */
            },
            "nightmare": "",
            "warmind": "",
            "chargedwithlight": "",
            "well": ""
        },
        "arms": {
            "rule": "",
            "general": "",
            "item": ["", ""],
            "raid": {
                "vog": "",
                "lastwish": "",
                "gos": "",
                "dsc": "",
                "votd": "",
            },
            "nightmare": "",
            "warmind": "",
            "chargedwithlight": "",
            "well": ""
        },
        "chest": {
            "rule": "",
            "general": "",
            "item": ["", ""],
            "raid": {
                "vog": "",
                "lastwish": "",
                "gos": "",
                "dsc": "",
                "votd": "",
            },
            "nightmare": "",
            "warmind": "",
            "chargedwithlight": "",
            "well": ""
        },
        "legs": {
            "rule": "",
            "general": "",
            "item": ["", ""],
            "raid": {
                "vog": "",
                "lastwish": "",
                "gos": "",
                "dsc": "",
                "votd": "",
            },
            "nightmare": "",
            "warmind": "",
            "chargedwithlight": "",
            "well": ""
        },
        "class": {
            "rule": "",
            "general": "",
            "item": ["", ""],
            "raid": {
                "vog": "",
                "lastwish": "",
                "gos": "",
                "dsc": "",
                "votd": "",
            },
            "nightmare": "",
            "warmind": "",
            "chargedwithlight": "",
            "well": ""
        },
        "unassigned": {
            "rule": "",
            "general": "",
            "raid": {
                "vog": "",
                "lastwish": "",
                "gos": "",
                "dsc": "",
                "votd": "",
            },
            "nightmare": "",
            "warmind": "",
            "chargedwithlight": "",
            "well": ""
        }
    }
}
```

[1] this requires something else: a fireteam view in DIM. I'm thinking a sidebar, much like the Item Feed, but on the left, that shows a quick view of everyone in your fireteam. The leader of the fireteam can "enforce" a ruleset (the button for that would replace the "apply loadout" button whnyou have at least one other person in your fireteam; otherwise it would be a "check" button that tells you whether you meet that ruleset). Once a ruleset is enforced, the fireteam view automatically opens (this would be toggleable in settings) and an icon on each player would display whether or not they meet the ruleset. If they do, for instance, a checkmark would appear on the right of their userbar, if they don't a red "X", and if they're not on DIM, then a yellow "!" in a triangle.  
