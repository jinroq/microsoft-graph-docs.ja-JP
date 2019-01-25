---
title: securityNetworkProtocol 列挙型
description: ネットワーク プロトコルの使用可能な値です。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511472"
---
# <a name="securitynetworkprotocol-enum"></a>securityNetworkProtocol 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ネットワーク プロトコルの使用可能な値です。

## <a name="members"></a>メンバー

|メンバー|値|説明|
|:---|:---|:---|
|不明|-1|不明なプロトコルです。|
|IP|(0)|インターネット プロトコルです。|
|icmp|-1| インターネット制御メッセージ プロトコル。|
|igmp|-2| インターネット グループ管理プロトコルです。|
|ggp|-3| ゲートウェイ間プロトコル。|
|ipv4|-4| インターネット プロトコル バージョン 4 です。|
|tcp|-6| 伝送制御プロトコル。|
|pup|1.2| まだ珍しかったころ汎用パケットのプロトコルです。|
|udp|1.7| ユーザー データグラム プロトコルです。|
|idp|2.2| インターネット データグラム プロトコルです。|
|ipv6|4.1| インターネット プロトコル バージョン 6 (ipv6) です。|
|ipv6RoutingHeader|4.3| ipv6 ルーティング ヘッダー。|
|ipv6FragmentHeader|4.4| ipv6 フラグメント ヘッダー。|
|ipSecEncapsulatingSecurityPayload|-50| ipv6 カプセル化セキュリティ ペイロード ヘッダー。|
|ipSecAuthenticationHeader|5.1| ipv6 認証ヘッダー。|
|icmpV6|5.8| Ipv6 用インターネット コントロール メッセージ プロトコル。|
|ipv6NoNextHeader|5.9| ipv6 次ヘッダーなし。|
|ipv6DestinationOptions|-60| ipv6 終点オプション ヘッダー。|
|nd|7.7| ネット ディスク プロトコル (非公式) です。|
|Raw|255| 生の IP パケットのプロトコルです。|
|ipx|-1000| インターネット パケット交換プロトコル。|
|spx|1256| シーケンスのパケット交換プロトコル。|
|spxII|1257| パケット交換バージョン 2 のプロトコル シーケンスが付けられました。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
