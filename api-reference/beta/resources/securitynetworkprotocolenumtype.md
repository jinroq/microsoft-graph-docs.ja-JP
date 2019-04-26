---
title: securitynetworkprotocol 列挙型
description: ネットワークプロトコルに指定できる値。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572452"
---
# <a name="securitynetworkprotocol-enum"></a>securitynetworkprotocol 列挙型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ネットワークプロトコルに指定できる値。

## <a name="members"></a>メンバー

|メンバー|値|説明|
|:---|:---|:---|
|不明|-1|不明なプロトコル。|
|ip|.0|インターネットプロトコル。|
|パケット|1 | インターネットコントロールメッセージプロトコル。|
|igmp|2 | インターネットグループ管理プロトコル。|
|ggp|3 | ゲートウェイからゲートウェイへのプロトコル。|
|ipv4|4 | インターネットプロトコルバージョン4。|
|tcp|6 | 伝送制御プロトコル。|
|.pup|12 | parc ユニバーサルパケットプロトコル。|
|受信|17 | ユーザーデータグラムプロトコル。|
|idp|×| インターネットデータグラムプロトコル。|
|ipv6|41| インターネットプロトコルバージョン 6 (ipv6)。|
|ipv6RoutingHeader|43| ipv6 ルーティングヘッダー。|
|ipv6FragmentHeader|44| ipv6 フラグメントヘッダー。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 カプセル化セキュリティペイロードヘッダー。|
|ipsecauthenticationheader|51| ipv6 認証ヘッダー。|
|過大|58| ipv6 のインターネット制御メッセージプロトコル。|
|ipv6NoNextHeader|59| ipv6 の次のヘッダーはありません。|
|ipv6DestinationOptions|60| ipv6 宛先オプションヘッダー。|
|目|77| ネットディスクプロトコル (非公式)。|
|時|255| 生の IP パケットプロトコル。|
|ipx|1000| インターネットパケット交換プロトコル。|
|spx|1256| 順序付きパケット交換プロトコル。|
|spxii|1257| シーケンス付きパケット交換バージョン2プロトコル。|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
