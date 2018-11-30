---
title: securityNetworkProtocol 列挙型
description: ネットワーク プロトコルの使用可能な値です。
ms.openlocfilehash: c0d676bc8c03faeee5ce8cf3265991304de31766
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021119"
---
# <a name="securitynetworkprotocol-enum-type"></a>securityNetworkProtocol 列挙型

ネットワーク プロトコルの使用可能な値です。

## <a name="members"></a>メンバー

|メンバー|値|説明|
|:---|:---|:---|
|不明|-1|不明なプロトコルです。|
|ip|0|インターネット プロトコルです。|
|icmp|1| インターネット制御メッセージ プロトコル。|
|igmp|2| インターネット グループ管理プロトコルです。|
|ggp|3| ゲートウェイ間プロトコル。|
|ipv4|4| インターネット プロトコル バージョン 4 です。|
|tcp|6| 伝送制御プロトコル。|
|pup|12| まだ珍しかったころ汎用パケットのプロトコルです。|
|udp|17| ユーザー データグラム プロトコルです。|
|idp|22| インターネット データグラム プロトコルです。|
|ipv6|41| インターネット プロトコル バージョン 6 (ipv6) です。|
|ipv6RoutingHeader|43| ipv6 ルーティング ヘッダー。|
|ipv6FragmentHeader|44| ipv6 フラグメント ヘッダー。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 カプセル化セキュリティ ペイロード ヘッダー。|
|ipSecAuthenticationHeader|51| ipv6 認証ヘッダー。|
|icmpV6|58| Ipv6 用インターネット コントロール メッセージ プロトコル。|
|ipv6NoNextHeader|59| ipv6 次ヘッダーなし。|
|ipv6DestinationOptions|60| ipv6 終点オプション ヘッダー。|
|nd|77| ネット ディスク プロトコル (非公式) です。|
|生|255| 生の IP パケットのプロトコルです。|
|ipx|1000| インターネット パケット交換プロトコル。|
|spx|1256| シーケンスのパケット交換プロトコル。|
|spxII|1257| パケット交換バージョン 2 のプロトコル シーケンスが付けられました。|