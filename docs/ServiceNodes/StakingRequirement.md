# Staking Requirement

A stake involves holding a specific cryptocoin in a wallet for a particular period of time. A staking requirement is the minimum amount of said cryptocoin that is required to stake.

## Service Node Staking Requirement
A Loki staking Requirement is the collateral requirement an operator stakes through a time-locked output which unlocks after a minimum of 21,600 blocks have elapsed (approximately 30 days). In the extra field of the transaction, the Service Node operator includes the Loki address which may receive Service Node rewards. This address will also be used as the public key for Service Node operations such as [swarm](../Advanced/SwarmFlagging.md) voting.

Before each node joins the Service Node network, other nodes must individually validate that the said nodes collateral outlay matches the required amount, as per the decreasing collateralisation requirement. Although collateral transactions  expire after 30 days, the wallet will have an opt-in automatic re-collateralisation feature.

The staking requirement started at 45,000 during Service Node launch (block height 101250), descends non-linearly to ~10,000 by year 4 (block height 1036800), and increases linearly to 15,000 by year 14 (block height 3628800), according to the equation:
![LSR](../assets/LSRformula.JPG)
Where *LSR* is the Loki Staking Requirement, *max* is the maximum value of two formulas, *min* is the minimum of two formulas, and *h* is the block height.
![Staking Requirement](../assets/StakingRequirement.JPG)

### LSR at Specific Dates
<details>
  <summary>Click to expand data </summary>
  
| Date (MM/YYYY)| Block Height|Staking Requirement (Loki)|
|:---------:|:---------:|:---------------:|
| 09/2018 | 101250  | 45000               |
| 10/2018 | 122850  | 41181               |
| 11/2018 | 144450  | 37780               |
| 12/2018 | 166050  | 34749               |
| 01/2019 | 187650  | 32049               |
| 02/2019 | 209250  | 29643               |
| 03/2019 | 230850  | 27500               |
| 04/2019 | 252450  | 25591               |
| 05/2019 | 274050  | 23890               |
| 06/2019 | 295650  | 22374               |
| 07/2019 | 317250  | 21024               |
| 08/2019 | 338850  | 19822               |
| 09/2019 | 360450  | 18750               |
| 10/2019 | 382050  | 17795               |
| 11/2019 | 403650  | 16945               |
| 12/2019 | 425250  | 16187               |
| 01/2020 | 446850  | 15512               |
| 02/2020 | 468450  | 14911               |
| 03/2020 | 490050  | 14375               |
| 04/2020 | 511650  | 13898               |
| 05/2020 | 533250  | 13472               |
| 06/2020 | 554850  | 13094               |
| 07/2020 | 576450  | 12756               |
| 08/2020 | 598050  | 12455               |
| 09/2020 | 619650  | 12188               |
| 10/2020 | 641250  | 11949               |
| 11/2020 | 662850  | 11736               |
| 12/2020 | 684450  | 11547               |
| 01/2021 | 706050  | 11378               |
| 02/2021 | 727650  | 11228               |
| 03/2021 | 749250  | 11094               |
| 04/2021 | 770850  | 10974               |
| 05/2021 | 792450  | 10868               |
| 06/2021 | 814050  | 10773               |
| 07/2021 | 835650  | 10689               |
| 08/2021 | 857250  | 10614               |
| 09/2021 | 878850  | 10547               |
| 10/2021 | 900450  | 10487               |
| 11/2021 | 922050  | 10434               |
| 12/2021 | 943650  | 10387               |
| 01/2022 | 965250  | 10345               |
| 02/2022 | 986850  | 10307               |
| 03/2022 | 1008450 | 10273               |
| 04/2022 | 1030050 | 10244               |
| 05/2022 | 1051650 | 10217               |
| 06/2022 | 1073250 | 10193               |
| 07/2022 | 1094850 | 10172               |
| 08/2022 | 1116450 | 10154               |
| 09/2022 | 1138050 | 10195               |
| 10/2022 | 1159650 | 10237               |
| 11/2022 | 1181250 | 10279               |
| 12/2022 | 1202850 | 10320               |
| 01/2023 | 1224450 | 10362               |
| 02/2023 | 1246050 | 10404               |
| 03/2023 | 1267650 | 10445               |
| 04/2023 | 1289250 | 10487               |
| 05/2023 | 1310850 | 10529               |
| 06/2023 | 1332450 | 10570               |
| 07/2023 | 1354050 | 10612               |
| 08/2023 | 1375650 | 10654               |
| 09/2023 | 1397250 | 10695               |
| 10/2023 | 1418850 | 10737               |
| 11/2023 | 1440450 | 10779               |
| 12/2023 | 1462050 | 10820               |
| 01/2024 | 1483650 | 10862               |
| 02/2024 | 1505250 | 10904               |
| 03/2024 | 1526850 | 10945               |
| 04/2024 | 1548450 | 10987               |
| 05/2024 | 1570050 | 11029               |
| 06/2024 | 1591650 | 11070               |
| 07/2024 | 1613250 | 11112               |
| 08/2024 | 1634850 | 11154               |
| 09/2024 | 1656450 | 11195               |
| 10/2024 | 1678050 | 11237               |
| 11/2024 | 1699650 | 11279               |
| 12/2024 | 1721250 | 11320               |
| 01/2025 | 1742850 | 11362               |
| 02/2025 | 1764450 | 11404               |
| 03/2025 | 1786050 | 11445               |
| 04/2025 | 1807650 | 11487               |
| 05/2025 | 1829250 | 11529               |
| 06/2025 | 1850850 | 11570               |
| 07/2025 | 1872450 | 11612               |
| 08/2025 | 1894050 | 11654               |
| 09/2025 | 1915650 | 11695               |
| 10/2025 | 1937250 | 11737               |
| 11/2025 | 1958850 | 11779               |
| 12/2025 | 1980450 | 11820               |
| 01/2026 | 2002050 | 11862               |
| 02/2026 | 2023650 | 11904               |
| 03/2026 | 2045250 | 11945               |
| 04/2026 | 2066850 | 11987               |
| 05/2026 | 2088450 | 12029               |
| 06/2026 | 2110050 | 12070               |
| 07/2026 | 2131650 | 12112               |
| 08/2026 | 2153250 | 12154               |
| 09/2026 | 2174850 | 12195               |
| 10/2026 | 2196450 | 12237               |
| 11/2026 | 2218050 | 12279               |
| 12/2026 | 2239650 | 12320               |
| 01/2027 | 2261250 | 12362               |
| 02/2027 | 2282850 | 12404               |
| 03/2027 | 2304450 | 12445               |
| 04/2027 | 2326050 | 12487               |
| 05/2027 | 2347650 | 12529               |
| 06/2027 | 2369250 | 12570               |
| 07/2027 | 2390850 | 12612               |
| 08/2027 | 2412450 | 12654               |
| 09/2027 | 2434050 | 12695               |
| 10/2027 | 2455650 | 12737               |
| 11/2027 | 2477250 | 12779               |
| 12/2027 | 2498850 | 12820               |
| 01/2028 | 2520450 | 12862               |
| 02/2028 | 2542050 | 12904               |
| 03/2028 | 2563650 | 12945               |
| 04/2028 | 2585250 | 12987               |
| 05/2028 | 2606850 | 13029               |
| 06/2028 | 2628450 | 13070               |
| 07/2028 | 2650050 | 13112               |
| 08/2028 | 2671650 | 13154               |
| 09/2028 | 2693250 | 13195               |
| 10/2028 | 2714850 | 13237               |
| 11/2028 | 2736450 | 13279               |
| 12/2028 | 2758050 | 13320               |
| 01/2029 | 2779650 | 13362               |
| 02/2029 | 2801250 | 13404               |
| 03/2029 | 2822850 | 13445               |
| 04/2029 | 2844450 | 13487               |
| 05/2029 | 2866050 | 13529               |
| 06/2029 | 2887650 | 13570               |
| 07/2029 | 2909250 | 13612               |
| 08/2029 | 2930850 | 13654               |
| 09/2029 | 2952450 | 13695               |
| 10/2029 | 2974050 | 13737               |
| 11/2029 | 2995650 | 13779               |
| 12/2029 | 3017250 | 13820               |
| 01/2030 | 3038850 | 13862               |
| 02/2030 | 3060450 | 13904               |
| 03/2030 | 3082050 | 13945               |
| 04/2030 | 3103650 | 13987               |
| 05/2030 | 3125250 | 14029               |
| 06/2030 | 3146850 | 14070               |
| 07/2030 | 3168450 | 14112               |
| 08/2030 | 3190050 | 14154               |
| 09/2030 | 3211650 | 14195               |
| 10/2030 | 3233250 | 14237               |
| 11/2030 | 3254850 | 14279               |
| 12/2030 | 3276450 | 14320               |
| 01/2031 | 3298050 | 14362               |
| 02/2031 | 3319650 | 14404               |
| 03/2031 | 3341250 | 14445               |
| 04/2031 | 3362850 | 14487               |
| 05/2031 | 3384450 | 14529               |
| 06/2031 | 3406050 | 14570               |
| 07/2031 | 3427650 | 14612               |
| 08/2031 | 3449250 | 14654               |
| 09/2031 | 3470850 | 14695               |
| 10/2031 | 3492450 | 14737               |
| 11/2031 | 3514050 | 14779               |
| 12/2031 | 3535650 | 14820               |
| 01/2032 | 3557250 | 14862               |
| 02/2032 | 3578850 | 14904               |
| 03/2032 | 3600450 | 14945               |
| 04/2032 | 3622050 | 14987               |
| 05/2032 | 3643650 | 15000               |
| 06/2032 | 3665250 | 15000               |
| 07/2032 | 3686850 | 15000               |
| 08/2032 | 3708450 | 15000               |
| 09/2032 | 3730050 | 15000               |
| 10/2032 | 3751650 | 15000               |
| 11/2032 | 3773250 | 15000               |
| 12/2032 | 3794850 | 15000               |

</details>