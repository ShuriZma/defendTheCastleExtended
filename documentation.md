# Variables

## Global

| Position | Variable                                                                                                                      | Description                                                                                                                                                 |
|----------|-------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 0        | <a name="gatePosition" style="all: unset">gatePosition</a>                                                                    | Defines the position of the gate                                                                                                                            |
| 1        | <a name="zenSpawnPositions" style="all: unset">zenSpawnPositions</a><sup>[2](#spawnPositions)</sup>                           | Counter used for increasing the possible spawn positions over time                                                                                          |
| 3        | <a name="loopIterator" style="all: unset">loopIterator</a>                                                                    | Used as counter for the current iteration of a loop                                                                                                         |
| 4        | <a name="bigBossSpawnPositions" style="all: unset">bigBossSpawnPositions</a><sup>[2](#spawnPositions)</sup>                   | Defines the possible spawn positions for Orisa                                                                                                              |
| 5        | <a name="playerSpawnPositions" style="all: unset">playerSpawnPositions</a><sup>[2](#spawnPositions)</sup>                     | Defines the possible spawn positions for players                                                                                                            |
| 6        | <a name="gateHealthChase" style="all: unset">gateHealthChase</a>                                                              | Variable being chased in order to show the gate health bar                                                                                                  |
| 7        | <a name="gateHealth" style="all: unset">gateHealth</a>                                                                        | Current gate health                                                                                                                                         |
| 8        | <a name="gateMaxHealth" style="all: unset">gateMaxHealth</a>                                                                  | Max gate health                                                                                                                                             |
| 9        | <a name="gateProgressBarColorCurrent" style="all: unset">gateProgressBarColorCurrent</a>                                      | Contains the current color the gate health bar is supposed to have                                                                                          |
| 10       | <a name="gateProgressBarColorComponent" style="all: unset">gateProgressBarColorComponent</a>                                  | Used to calculate the gateProgressBarColorCurrent                                                                                                           |
| 11       | <a name="gateHealthEvent" style="all: unset">gateHealthEvent</a>                                                              | Contains the amount of health the gate has on the last event                                                                                                |
| 12       | <a name="bastionTargetPositions" style="all: unset">bastionTargetPositions</a><sup>[1](#targetPositions)</sup>                | Defines target positions for Bastion                                                                                                                        |
| 13       | <a name="sniperPositions" style="all: unset">sniperPositions</a><sup>[2](#spawnPositions)</sup>                               | Defines spawn Positions for Widowmaker                                                                                                                      |
| 14       | <a name="ballSpawnPositions" style="all: unset">ballSpawnPositions</a><sup>[2](#spawnPositions)</sup>                         | Defines spawn Positions for Wreckingball                                                                                                                    |
| 15       | <a name="zenRespawnTime" style="all: unset">zenRespawnTime</a>                                                                | Defines Zenyattas respawn time                                                                                                                              |
| 16       | <a name="timeSeconds" style="all: unset">timeSeconds</a>                                                                      | Contains the seconds part of the match timer                                                                                                                |
| 17       | <a name="timeMinutes" style="all: unset">timeMinutes</a>                                                                      | Contains the minutes part of the match timer                                                                                                                |
| 18       | <a name="defaultCurrentBot" style="all: unset">defaultCurrentBot</a>                                                          | Contains the bot that will be destroyed/replaced next<br>Might be renamed soon                                                                              |
| 19       | <a name="defaultHeroBotsPool" style="all: unset">defaultHeroBotsPool</a>                                                      | Defines the heroes being played by ai<br>Code around this could need some serious rework<br>Hukuta left us with a bunch of seriously unnecessary complexity |
| 20       | <a name="defaultHeroBotsPoolCurrentId" style="all: unset">defaultHeroBotsPoolCurrentId</a>                                    | This is pretty much just an iteration counter for defaultHeroBotsPool                                                                                       |
| 21       | <a name="isDebug" style="all: unset">isDebug</a>                                                                              | Determines if the debug mode is active                                                                                                                      |
| 22       | <a name="botOrisaParent" style="all: unset">botOrisaParent</a>                                                                | Contains the current Orisa Dummy                                                                                                                            |
| 24       | <a name="botOrisaChild" style="all: unset">botOrisaChild</a>                                                                  | Contains the current Bastion Dummy being stuck onto botOrisaParent                                                                                          |
| 25       | <a name="gateRepairPosition" style="all: unset">gateRepairPosition</a>                                                        | Defines the position you have to look at when trying to repair the gate                                                                                     |
| 26       | <a name="botOrisaTargetPosition" style="all: unset">botOrisaTargetPosition</a><sup>[1](#targetPositions)</sup>                | Defines the target position for Orisa                                                                                                                       |
| 27       | <a name="botEchoRespawnPosition" style="all: unset">botEchoRespawnPosition</a><sup>[2](#spawnPositions)</sup>                 | Defines the spawn/portal position for Echo                                                                                                                  |
| 28       | <a name="botEchoTeleportPositions" style="all: unset">botEchoTeleportPositions                                                | Defines the player teleport positions for Echo                                                                                                              |
| 29       | <a name="upgradeGateMaxHealthValue" style="all: unset">upgradeGateMaxHealthValue</a><sup>[3](#teamChallenges)</sup>           | Contains the current amount of repaired gate health                                                                                                         |
| 30       | <a name="upgradeGateMaxHealthHudId" style="all: unset">upgradeGateMaxHealthHudId</a><sup>[3](#teamChallenges)</sup>           | Contains the challenge HUD                                                                                                                                  |
| 31       | <a name="upgradePlayerMaxHealthValue" style="all: unset">upgradePlayerMaxHealthValue</a><sup>[3](#teamChallenges)</sup>       | Contains the current amount of healed player health                                                                                                         |
| 32       | <a name="upgradePlayerMaxHealthHudId" style="all: unset">upgradePlayerMaxHealthHudId</a><sup>[3](#teamChallenges)</sup>       | Contains the challenge HUD                                                                                                                                  |
| 33       | <a name="upgradeCriticalDamageValue" style="all: unset">upgradeCriticalDamageValue</a><sup>[3](#teamChallenges)</sup>         | Contains the current amount Widowmaker/Echo kills                                                                                                           |
| 34       | <a name="upgradeCriticalDamageHudId" style="all: unset">upgradeCriticalDamageHudId</a><sup>[3](#teamChallenges)</sup>         | Contains the challenge HUD                                                                                                                                  |
| 35       | <a name="upgradeMaxAmmoValue" style="all: unset">upgradeMaxAmmoValue</a><sup>[3](#teamChallenges)</sup>                       | Contains the current amount of Zenyatta kills                                                                                                               |
| 36       | <a name="upgradeMaxAmmoHudId" style="all: unset">upgradeMaxAmmoHudId</a><sup>[3](#teamChallenges)</sup>                       | Contains the challenge HUD                                                                                                                                  |
| 37       | <a name="upgradeMaxAmmoMaxValue" style="all: unset">upgradeMaxAmmoMaxValue</a><sup>[3](#teamChallenges)</sup>                 | Contains the value needed to finish the challenge                                                                                                           |
| 38       | <a name="upgradePlayerMaxHealthMaxValue" style="all: unset">upgradePlayerMaxHealthMaxValue</a><sup>[3](#teamChallenges)</sup> | Contains the value needed to finish the challenge                                                                                                           |
| 39       | <a name="upgradePlayerMaxHealthMaxValue" style="all: unset">upgradePlayerMaxHealthMaxValue</a><sup>[3](#teamChallenges)</sup> | Contains the value needed to finish the challenge                                                                                                           |
| 40       | <a name="upgradeGateMaxHealthMaxValue" style="all: unset">upgradeGateMaxHealthMaxValue</a><sup>[3](#teamChallenges)</sup>     | Contains the value needed to finish the challenge                                                                                                           |
| 41       | <a name="damageBoost" style="all: unset">damageBoost</a>                                                                      | Contains the damage % that is being put on top of the base damage                                                                                           |
| 42       | <a name="isDebugAINavigation" style="all: unset">isDebugAINavigation</a>                                                      |                                                                                                                                                             |
| 43       | <a name="gameLogicCountOfUniqueHeroes" style="all: unset">gameLogicCountOfUniqueHeroes</a>                                    |                                                                                                                                                             |
| 44       | <a name="isNewWaveGameLogicProcessing" style="all: unset">isNewWaveGameLogicProcessing</a>                                    |                                                                                                                                                             |
| 45       | <a name="automaticRepair" style="all: unset">automaticRepair</a>                                                              |                                                                                                                                                             |
| 46       | <a name="upgradePerkSharpshooterValue" style="all: unset">upgradePerkSharpshooterValue</a>                                    |                                                                                                                                                             |
| 47       | <a name="perk" style="all: unset">perk</a>                                                                                    |                                                                                                                                                             |
| 48       | <a name="maxHealthDone" style="all: unset">maxHealthDone</a>                                                                  |                                                                                                                                                             |
| 49       | <a name="startMoney" style="all: unset">startMoney</a>                                                                        |                                                                                                                                                             |
| 50       | <a name="time5Minutes" style="all: unset">time5Minutes</a>                                                                    |                                                                                                                                                             |
| 51       | <a name="selfNanoWorkshopSetting" style="all: unset">selfNanoWorkshopSetting</a>                                              |                                                                                                                                                             |
| 52       | <a name="shopCamPosition" style="all: unset">shopCamPosition</a>                                                              |                                                                                                                                                             |
| 53       | <a name="shopBasePosition" style="all: unset">shopBasePosition</a>                                                            |                                                                                                                                                             |
| 54       | <a name="shopPositionAngle" style="all: unset">shopPositionAngle</a>                                                          |                                                                                                                                                             |
| 55       | <a name="activeBoss" style="all: unset">activeBoss</a>                                                                        |                                                                                                                                                             |
| 57       | <a name="bossRotation" style="all: unset">bossRotation</a>                                                                    |                                                                                                                                                             |
| 58       | <a name="lastBoss" style="all: unset">lastBoss</a>                                                                            |                                                                                                                                                             |
| 59       | <a name="time10Minutes" style="all: unset">time10Minutes</a>                                                                  |                                                                                                                                                             |
| 60       | <a name="moneyMultiplier" style="all: unset">moneyMultiplier</a>                                                              |                                                                                                                                                             |
| 61       | <a name="challengeCount" style="all: unset">challengeCount</a>                                                                |                                                                                                                                                             |
| 62       | <a name="upgradeBossHealthValue" style="all: unset">upgradeBossHealthValue</a>                                                |                                                                                                                                                             |
| 63       | <a name="globalHUDs" style="all: unset">globalHUDs</a>                                                                        |                                                                                                                                                             |
| 64       | <a name="baseStats" style="all: unset">baseStats</a>                                                                          |                                                                                                                                                             |
| 112      | <a name="allPositions" style="all: unset">allPositions</a>                                                                    |                                                                                                                                                             |
| 113      | <a name="allDirections" style="all: unset">allDirections</a>                                                                  |                                                                                                                                                             |
| 114      | <a name="firstPosition" style="all: unset">firstPosition</a>                                                                  |                                                                                                                                                             |
| 115      | <a name="secondPosition" style="all: unset">secondPosition</a>                                                                |                                                                                                                                                             |
| 116      | <a name="firstPoint" style="all: unset">firstPoint</a>                                                                        |                                                                                                                                                             |
| 117      | <a name="secondPoint" style="all: unset">secondPoint</a>                                                                      |                                                                                                                                                             |
| 118      | <a name="second" style="all: unset">second</a>                                                                                |                                                                                                                                                             |
| 119      | <a name="z" style="all: unset">z</a>                                                                                          |                                                                                                                                                             |
| 120      | <a name="wallId" style="all: unset">wallId</a>                                                                                |                                                                                                                                                             |
| 121      | <a name="showWalls" style="all: unset">showWalls</a>                                                                          |                                                                                                                                                             |
| 122      | <a name="isGrounded" style="all: unset">isGrounded</a>                                                                        |                                                                                                                                                             |
| 123      | <a name="beamType" style="all: unset">beamType</a>                                                                            |                                                                                                                                                             |
| 125      | <a name="nodePositions" style="all: unset">nodePositions</a>                                                                  |                                                                                                                                                             |
| 126      | <a name="nodeConnections" style="all: unset">nodeConnections</a>                                                              |                                                                                                                                                             |
| 127      | <a name="distanceMatrix" style="all: unset">distanceMatrix</a>                                                                |                                                                                                                                                             |

> <a name="targetPositions" style="all: unset">1</a>: Target position variables can pretty much be merged
>
> <a name="spawnPositions" style="all: unset">2</a>: Spawn position variables can pretty much be merged
>
> <a name="teamChallenges" style="all: unset">3</a>: upgrade* variables can be merged into one

## Player
| Position | Variable                                                                                           | Description |
|----------|----------------------------------------------------------------------------------------------------|-------------|
| 0        | <a name="botSeePlayer" style="all: unset">botSeePlayer</a>                                         |             |
| 1        | <a name="botDoesUniqueBehaviour" style="all: unset">botDoesUniqueBehaviour</a>                     |             |
| 2        | <a name="botEffects" style="all: unset">botEffects</a>                                             |             |
| 3        | <a name="botRayCastHitPosition" style="all: unset">botRayCastHitPosition</a>                       |             |
| 4        | <a name="botEventPosition" style="all: unset">botEventPosition</a>                                 |             |
| 5        | <a name="currentHero" style="all: unset">currentHero</a>                                           |             |
| 6        | <a name="isDead" style="all: unset">isDead</a>                                                     |             |
| 7        | <a name="isRespawning" style="all: unset">isRespawning</a>                                         |             |
| 8        | <a name="botBastionArtilleryDidShotsCount" style="all: unset">botBastionArtilleryDidShotsCount</a> |             |
| 9        | <a name="botCounter" style="all: unset">botCounter</a>                                             |             |
| 10       | <a name="hasBadStatus" style="all: unset">hasBadStatus</a>                                         |             |
| 11       | <a name="eventHealth" style="all: unset">eventHealth</a>                                           |             |
| 12       | <a name="healOverTimeId" style="all: unset">healOverTimeId</a>                                     |             |
| 13       | <a name="botIsOrisaChild" style="all: unset">botIsOrisaChild</a>                                   |             |
| 14       | <a name="botEchoCapturedPlayer" style="all: unset">botEchoCapturedPlayer</a>                       |             |
| 15       | <a name="botPlayersInRadius" style="all: unset">botPlayersInRadius</a>                             |             |
| 16       | <a name="botLoopIterator2" style="all: unset">botLoopIterator2</a>                                 |             |
| 17       | <a name="botWidowShotTime" style="all: unset">botWidowShotTime</a>                                 |             |
| 18       | <a name="botWidowTeleportTime" style="all: unset">botWidowTeleportTime</a>                         |             |
| 19       | <a name="isNanoed" style="all: unset">isNanoed</a>                                                 |             |
| 20       | <a name="abilityHUD" style="all: unset">abilityHUD</a>                                             |             |
| 21       | <a name="lucioDashActive" style="all: unset">lucioDashActive</a>                                   |             |
| 22       | <a name="lucioDashIcon" style="all: unset">lucioDashIcon</a>                                       |             |
| 23       | <a name="anaEntityID" style="all: unset">anaEntityID</a>                                           |             |
| 24       | <a name="abilities" style="all: unset">abilities</a>                                               |             |
| 25       | <a name="money" style="all: unset">money</a>                                                       |             |
| 26       | <a name="heroTalentText" style="all: unset">heroTalentText</a>                                     |             |
| 27       | <a name="damageBoost" style="all: unset">damageBoost</a>                                           |             |
| 28       | <a name="playerHealth" style="all: unset">playerHealth</a>                                         |             |
| 29       | <a name="abilityCountdown" style="all: unset">abilityCountdown</a>                                 |             |
| 30       | <a name="hpPool" style="all: unset">hpPool</a>                                                     |             |
| 31       | <a name="effects" style="all: unset">effects</a>                                                   |             |
| 32       | <a name="abilityProjectile" style="all: unset">abilityProjectile</a>                               |             |
| 33       | <a name="abilityEnd" style="all: unset">abilityEnd</a>                                             |             |
| 34       | <a name="abilityAvailable" style="all: unset">abilityAvailable</a>                                 |             |
| 35       | <a name="moveSpeed" style="all: unset">moveSpeed</a>                                               |             |
| 36       | <a name="damageMod" style="all: unset">damageMod</a>                                               |             |
| 37       | <a name="critDamageBoost" style="all: unset">critDamageBoost</a>                                   |             |
| 38       | <a name="soldierEspionage" style="all: unset">soldierEspionage</a>                                 |             |
| 39       | <a name="healingDealt" style="all: unset">healingDealt</a>                                         |             |
| 41       | <a name="chainReactionOn" style="all: unset">chainReactionOn</a>                                   |             |
| 42       | <a name="chainReactionImmune" style="all: unset">chainReactionImmune</a>                           |             |
| 43       | <a name="abilityActive" style="all: unset">abilityActive</a>                                       |             |
| 45       | <a name="secondWindActive" style="all: unset">secondWindActive</a>                                 |             |
| 46       | <a name="isInMenu" style="all: unset">isInMenu</a>                                                 |             |
| 48       | <a name="playerFacing" style="all: unset">playerFacing</a>                                         |             |
| 49       | <a name="isBoss" style="all: unset">isBoss</a>                                                     |             |
| 53       | <a name="deathPosition" style="all: unset">deathPosition</a>                                       |             |
| 54       | <a name="lastSecondWind" style="all: unset">lastSecondWind</a>                                     |             |
| 55       | <a name="vote" style="all: unset">vote</a>                                                         |             |
| 105      | <a name="filterPosition" style="all: unset">filterPosition</a>                                     |             |
| 106      | <a name="lastSavedPosition" style="all: unset">lastSavedPosition</a>                               |             |
| 107      | <a name="closestBodyPosition" style="all: unset">closestBodyPosition</a>                           |             |
| 108      | <a name="fullBodyPosition" style="all: unset">fullBodyPosition</a>                                 |             |
| 109      | <a name="previousPositionIntersection" style="all: unset">previousPositionIntersection</a>         |             |
| 110      | <a name="activeWall" style="all: unset">activeWall</a>                                             |             |
| 111      | <a name="closestWall" style="all: unset">closestWall</a>                                           |             |
| 112      | <a name="x" style="all: unset">x</a>                                                               |             |
| 113      | <a name="intersectionLength" style="all: unset">intersectionLength</a>                             |             |
| 114      | <a name="thickness" style="all: unset">thickness</a>                                               |             |
| 115      | <a name="botCancelPathFinding" style="all: unset">botCancelPathFinding</a>                         |             |
| 116      | <a name="botLoopIterator1" style="all: unset">botLoopIterator1</a>                                 |             |
| 117      | <a name="botTempArray" style="all: unset">botTempArray</a>                                         |             |
| 118      | <a name="botTargetPlayer" style="all: unset">botTargetPlayer</a>                                   |             |
| 119      | <a name="botTargetPosition" style="all: unset">botTargetPosition</a>                               |             |
| 120      | <a name="botClosestNodeIdToTarget" style="all: unset">botClosestNodeIdToTarget</a>                 |             |
| 121      | <a name="botClosestNodeIdToBot" style="all: unset">botClosestNodeIdToBot</a>                       |             |
| 122      | <a name="botPreviousNodeId" style="all: unset">botPreviousNodeId</a>                               |             |
| 123      | <a name="botNextNodeId" style="all: unset">botNextNodeId</a>                                       |             |
| 124      | <a name="botNextNodePosition" style="all: unset">botNextNodePosition</a>                           |             |
| 125      | <a name="botCurrentDistanceToTarget" style="all: unset">botCurrentDistanceToTarget</a>             |             |
| 126      | <a name="botShortestDistanceToTarget" style="all: unset">botShortestDistanceToTarget</a>           |             |
| 127      | <a name="botIsPathFinding" style="all: unset">botIsPathFinding</a>                                 |             |


## Subroutine

| Position | Variable                                                                                 | Description |
|----------|------------------------------------------------------------------------------------------|-------------|
| 0        | <a name="BotBastionArtilleryDamage" style="all: unset">BotBastionArtilleryDamage</a>     |             |
| 2        | <a name="BotBastionRespawn" style="all: unset">BotBastionRespawn</a>                     |             |
| 3        | <a name="GateProgressBarColor" style="all: unset">GateProgressBarColor</a>               |             |
| 4        | <a name="BotZenyattaRespawn" style="all: unset">BotZenyattaRespawn</a>                   |             |
| 5        | <a name="BotWidowRespawn" style="all: unset">BotWidowRespawn</a>                         |             |
| 6        | <a name="BotBallRespawn" style="all: unset">BotBallRespawn</a>                           |             |
| 7        | <a name="GameLogicAddNextHeroInGame" style="all: unset">GameLogicAddNextHeroInGame</a>   |             |
| 8        | <a name="BotOrisaRespawn" style="all: unset">BotOrisaRespawn</a>                         |             |
| 9        | <a name="BotLandingFromSky" style="all: unset">BotLandingFromSky</a>                     |             |
| 10       | <a name="BotEchoRespawn" style="all: unset">BotEchoRespawn</a>                           |             |
| 11       | <a name="BotEchoDetachPlayer" style="all: unset">BotEchoDetachPlayer</a>                 |             |
| 12       | <a name="BotEchoFlyToPlayer" style="all: unset">BotEchoFlyToPlayer</a>                   |             |
| 13       | <a name="BotEchoFlyToPortal" style="all: unset">BotEchoFlyToPortal</a>                   |             |
| 14       | <a name="GameLogicSetBotProperties" style="all: unset">GameLogicSetBotProperties</a>     |             |
| 15       | <a name="DisablePlayer" style="all: unset">DisablePlayer</a>                             |             |
| 16       | <a name="BotAppearFromUnderground" style="all: unset">BotAppearFromUnderground</a>       |             |
| 17       | <a name="BotReinRespawn" style="all: unset">BotReinRespawn</a>                           |             |
| 18       | <a name="PlayerInit" style="all: unset">PlayerInit</a>                                   |             |
| 19       | <a name="BotInit" style="all: unset">BotInit</a>                                         |             |
| 20       | <a name="PlayerRespawn" style="all: unset">PlayerRespawn</a>                             |             |
| 21       | <a name="BotRespawn" style="all: unset">BotRespawn</a>                                   |             |
| 22       | <a name="BotWidowBadStatus" style="all: unset">BotWidowBadStatus</a>                     |             |
| 23       | <a name="GameLogicWave0" style="all: unset">GameLogicWave0</a>                           |             |
| 24       | <a name="Refund" style="all: unset">Refund</a>                                           |             |
| 25       | <a name="EnablePlayer" style="all: unset">EnablePlayer</a>                               |             |
| 26       | <a name="GateRepair" style="all: unset">GateRepair</a>                                   |             |
| 27       | <a name="CancelMomentum" style="all: unset">CancelMomentum</a>                           |             |
| 28       | <a name="UpdateDamage" style="all: unset">UpdateDamage</a>                               |             |
| 124      | <a name="BotStartPathFinding" style="all: unset">BotStartPathFinding</a>                 |             |
| 125      | <a name="BotGetClosestNodeIdToTarget" style="all: unset">BotGetClosestNodeIdToTarget</a> |             |
| 126      | <a name="BotGetNextNodeIdAndPosition" style="all: unset">BotGetNextNodeIdAndPosition</a> |             |
| 127      | <a name="BotResetPathFinding" style="all: unset">BotResetPathFinding</a>                 |             |
