# Economy

Players start with $500 and can earn more money by [voting](https://www.left4craft.org/vote/), trading with players, or participating in [count to a million](https://discord.com/channels/424571587413540874/779454172826697728) in the Discord server.

Trade can take take place either on the [public marketplace](#marketplace), or privately through [`/trade`](#trade).

## Earnings per action
| Action                     | Earnings |
| -------------------------- | -------- |
| Voting                     | $100     |
| Selling Item               | Varies   |
| Discord count to a million | $25      |

## Commands
| Command                  | Aliases   | Description                      |
| ------------------------ | --------- | -------------------------------- |
| `/balance [player]`      | `/bal`    | See how much money you have      |
| `/balancetop`            | `/baltop` | See who has the most money       |
| `/pay <player> <amount>` |           | Transfer money to another player |
| `/trade <player>`        |           | Trade with a player              |
| `/marketplace ...`       | `/mp ...` | Use the marketplace              |


### Marketplace

The virtual marketplace allows players to list items for sale at a set price which other players can buy, even when the seller is offline.

#### Commands

| Command                                                    | Description                                             |
| ---------------------------------------------------------- | ------------------------------------------------------- |
| `/mp publish/sell <price>`                                 | Sell the item in your hand                              |
| `/mp search`                                               | Open the search menu                                    |
| `/mp limits [get|decrement] [player] [slots]`              | Manage the limits of players                            |
| `/mp help [command]`                                       | Open the help menu or get help from a specific command. |
| `/mp cancel/borrow <options>`                              | Cancel items, for now just –all enabled                 |
| `/mp setpin/webpin <new-pin>`                              | Sets the pin of your webclient account.                 |
| `/mp wallet/webmoney <deposit|widthdraw|check> [player|$]` | Manage the money in your webclient account.             |

[More information.](https://marketplacedocs.readthedocs.io/en/latest/commands)

### Trade

The Trade GUI allows two players to safely exchange items, money, XP (experience points), and claim blocks. Neither player can take the other's items until both accept the trade.

Initiate trade with  `/trade <player>`. The other player will have 15 seconds to accept your trade offer by clicking in chat.