# Changelog

## v0.2.6

2022-05-24

- fix reconnect panic
- update spot and futures models
- add `ShowReconnectMsg` config field to decide to show reconnect success msg
- update some test cases

## v0.2.5

- update future's models, fix fields wrong type

## v0.2.4

2021-08-12

- update futures models, fix fields wrong type
- add futures model `FuturesPositions`

## v0.2.3

2021-08-11

- Support websocket skip tls verify with `SkipTlsVerify` of ConfOptions
- Update futures models
- Update examples

## v0.2.2

2021-07-23

- Add constant `ChannelSpotCrossBalance` support `spot.cross_balances` channel
- SpotUserTradesMsg add field `Text` for orders' text
- Update local order book example

## v0.2.1

2021-06-24

- fix futures book ticker and order book update struct

## v0.2.0

2021-06-24

- fix futures order book update struct

## v0.1.9

2021-06-24

- add futures order book struct

## v0.1.8

2021-06-22

- add `WsService` method `GetConnection()` to get the connection
- fix `changelog` date error

## v0.1.7

2021-06-04

- fix reconnect msg nil `SubscribeOptions` caused reconnect msg lost

## v0.1.6

2021-06-04

- add `io.ErrUnexpectedEOF` error capture, it caused v0.1.5 can't reconnect
- fix reconnect msg repeat add

## v0.1.5

2021-06-02

- add `SpotUpdateAllDepthMsg` struct for parse all order book msg

## v0.1.4

2021-06-02

- fix overlapping price for local order book example
- update README

## v0.1.3

2021-05-26

- Support futures websocket.
- Modify channels name to with flag `Spot` or `Future`.
- Add field `TimestampInMilli`  in models `SpotBalancesMsg`, `SpotFundingBalancesMsg`, `SpotMarginBalancesMsg`. Add
  field `TimeInMilli` in model `SpotBookTickerMsg`
- Add new method `NewConnConfFromOption` to get a ConnConf flexible.
- Add new method `SubscribeWithOption` to support futures subscribe with id.
- Add example for both spot and futures connection use.
- Fix reconnect websocket failed bug.
- Optimizing code structure.

## v0.1.2

2021-04-19

- Fix subscribe repeat bug.

## v0.1.1

2021-04-16

- Fix subscribe channel failed bug.

## v0.1.0

2021-04-12

- Support spot websocket function.