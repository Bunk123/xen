   getgenv().fraudfun = { -- fraud.fun = fraud.lol
        ['Startup'] = {
            Key = 'GGyUpCKwrxfIbpQgKxFmMQULrJYzrxgk', -- replace key here with your luarmor key
            Intro = true, -- shows an intro on startup
            GUI = true, -- enables the gui, will drop fps a little
            NotificationMode = "Roblox", -- roblox, default (default broken on solara)
            ['FPS'] = {
                UnlockFPS = true, -- unlocks your fps
                FpsCap = 9999, -- max fps 
            },
        },
        ['Panic'] = {
            Enabled = false, -- will disable all features
            Keybind = "P", -- panic keybind
            PanicNotifications = true, -- notifys if you panic
        },
        ['Silent Aim'] = {
            Enabled = true, -- enables silent aim
            Mode = "FOV", -- FOV (normal silent), Target
            TargetBind = "C", -- bind for target mode
            TargetNotifications = false, -- notifys you when changed target
            ['Prediction'] = {
                Prediction = 0.145235456, -- prediction value
                HitChance = 100, -- chance to hit your target (0-100)
            },
            ['Hitpart'] = {
                Hitpart = "HumanoidRootPart", -- HumanoidRootPart, UpperTorso, LowerTorso, Head
                ClosetPart = false, -- uses closet hitpart, all parts supported
            },
            ['Visuals'] = {
                Dot = false, -- adds a dot to the target
                Tracer = false, -- adds a tracer to the target
            },
        },
        ['Aimlock'] = {
            Enabled = true, -- enables camlock
            Mode = "Target", -- FOV, Target (normal aimlock)
            TargetBind = "C", -- bind for target mode
            TargetNotifications = false, -- notifys you when changed target
            ['Prediction'] = {
                Prediction = 0.14, -- prediction value
                HitChance = 100, -- chance to hit your target (0-100)
                EasingStyle = "Exponential", -- https://create.roblox.com/docs/reference/engine/enums/EasingStyle
            },
            ['Hitpart'] = {
                Hitpart = "HumanoidRootPart", -- HumanoidRootPart, UpperTorso, LowerTorso, Head
                ClosetPart = false, -- uses closet hitpart, all parts supported
            },
            ['Smoothness'] = {
                Enabled = true, -- smooths the camlock, looks legit
                Amount = 0.065, -- smoothing amount
            },
            ['Visuals'] = {
                Dot = false, -- adds a dot to the target
                Tracer = false, -- adds a tracer to the target
            },
            ['Shake'] = {
                Enabled = false, -- shakes your camera on the target
                X = 5, -- shake x position
                Y = 5, -- shake y position
                Z = 5, -- shake z position
            }
        },
        ['Global'] = {
            AutoPrediction = false, -- automatically sets a prediction based on your ping
            Predictions = { -- if you set here, it wont show on gui. your predictions will still work
                Ping30 = 0.1099,
                Ping40 = 0.1195,
                Ping50 = 0.1219,
                Ping60 = 0.1237,
                Ping70 = 0.1291,
                Ping80 = 0.1337,
                Ping90 = 0.1349,
                Ping100 = 0.1378,
                Ping110 = 0.1459,
                Ping120 = 0.149,
                Ping130 = 0.151,
                Ping140 = 0.1652131,
                Ping150 = 0.125333,
                Ping160 = 0.1223333,
                Ping170 = 0.15,
                Ping180 = 0.1923111,
                Ping190 = 0.165771,
                Ping200 = 0.1746,
            },
            AntiGroundShots = false, -- doesnt hit ground shots
            UnlockOnDeath = false, -- unlocks on target death
            UnlockOutsideFOV = false, -- unlocks if target outside of fov
            UnlockBehindWall = false, -- unlocks if target behind a wall
        },
        ['Checks'] = {
            VisibleCheck = true, -- wont lock on if player behind a wall
            DeathCheck = true, -- wont lock on if player is knocked or grabbed
            CrewCheck = false, -- wont lock on if player is in your crew
            FriendCheck  = false, -- wont lock on if player is added on roblox
                Distance = { -- wont lock if to far away
                Enabled = false,
                MaxDistance = 250, -- studs
            }
        },
        ['Resolver'] = {
            Enabled = false, -- resolve anti locks and desyncs
            Method = "Delta", -- Delta, Move Direction, No Prediction, Recalculate
            Keybind = false, -- toggles resolver with keybind below
            KeybindBind = "T", -- keybind to toggle resolver if enabled
        },
        ['FOV'] = { -- fov / circle settings
            SilentAim = {
                Visible = true, -- enables fov for silent aim
                Filled = false, -- fills fov
                Size = 75, -- size of fov
                Thickness = 1, -- thickness of fov
                Transparency = 0.1, -- transparency of fov (0.1 - 1)
                Color = Color3.fromRGB(0,0,0) -- fov color
            },
            Camlock = {
                Visible = false, -- enables fov for silent aim
                Filled = false, -- fills fov
                Size = 30, -- size of fov
                Thickness = 1, -- thickness of fov
                Transparency = 1, -- transparency of fov (0.1 - 1)
                Color = Color3.fromRGB(255,0,0) -- fov color
            },
        },
        ['Airshot'] = {
            Enabled = false, -- adjusts prediction if target is in air (beam niggas down)
            JumpOffset = -1.5, -- changes offset if target is in air
            Smoothness = { -- changes smoothness on target jump
                Enabled = true,
                JumpSmoothness = 0.5, -- smoothness while target is in air
            }
        },
        ['Macro'] = {
            Enabled = true, -- enable macro
            Bind = "X", -- macro bind
            FirstPerson = true, -- macro abuse
        },
        ['CustomCrosshair'] = {
            Enabled = true, -- toggles crosshair
            Mode = "mouse", -- center, mouse
            Visuals = {
                Width = 1.5,
                Length = 10,
                Radius = 11,
                Color = Color3.fromRGB(255,0,0),
            },
            Spin = {
                Enabled = true,
                SpinSpeed = 150,
                SpinMax = 340,
                SpinStyle = Enum.EasingStyle.Circular, -- Circular, Linear
            },
            Resize = {
                Enabled = false,
                ResizeSpeed = 150,
                ResizeMin = 5,
                ResizeMax = 22,
            }
        },
        ['OnHit'] = {
            HitSounds = {
                Enabled = false, -- enables hit sounds
                HitSound = "Rust", -- Bameware, Bubble, Rust, Neverlose, Skeet, Minecraft
                Volume = 1, -- hit sound volume
            },
            HitLog = {
                Enabled = false, -- notifys you when a target is hit
            }
        },
        ['MemorySpoofer'] = {
            Enabled = false, -- spoofs your memory, scripts increase memory on inject
            Min = 750,
            Max = 1000,
        },
        ['Extra'] = {
            DisableSeats = true, -- disable seats (helps macro and your mental health)
            LowGraphics = false, -- automatically sets low graphics
        },
        ['ESP'] = {
            Enabled = false, -- enables esp, will legit eat your fps like a fat nigga named caseoh
            Boxes = {
                Enabled = false, -- enables boxes
                BoxColor = Color3.fromRGB(0,0,0), -- box color
                Filled = false, -- filles boxes
                FilledBoxColor = Color3.fromRGB(255,255,255), -- box fill color
                HealthBar = false, -- health bar
            },
            Text = {
                Names = false, -- enables names
                Distance = false, -- enables player distances
                TextColor = Color3.fromRGB(255,255,255) -- text color
            },
            Tracer = {
                Enabled = false, -- enables tracers
                TracerOrigin = "Bottom", -- Bottom, Top, Mouse
                TracerColor = Color3.fromRGB(255,0,0),
            }
        }
    }
loadstring(game:HttpGet("https://raw.githubusercontent.com/angxlzz/dahood/main/fraudlol"))()
