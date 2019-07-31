---
title: userSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c0f9cb91484f23702329a38de26189176dacb13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964236"
---
# <a name="usersecuritystate-resource-type"></a>userSecurityState リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーアカウントに関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|Usersecuritystate|String|AAD User オブジェクト識別子 (GUID)-物理/マルチアカウントユーザーエンティティを表します。|
|accountName|String|ユーザーアカウントのアカウント名 (Active Directory ドメインまたは DNS ドメインなし)-(と`mailNickName`も呼ばれます)。|
|domainName|String|ユーザーアカウントの NetBIOS/Active Directory ドメイン (つまり、"ドメイン \ ユーザー名" の形式)。|
|emailRole|emailRole|電子メール関連の警告の場合-ユーザーアカウントの電子メール ' ロール '。 可能な値は、`unknown`、`sender`、`recipient` です。|
|isVpn|Boolean|ユーザーが VPN を介してログオンしたかどうかを示します。|
|logonDateTime|DateTimeOffset|サインインが発生した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|logonId|String|ユーザーのサインイン ID。|
|logonIp|String|サインイン要求の送信元の IP アドレス。|
|logonLocation|String|このユーザーによってユーザーのサインインイベントに関連付けられている場所 (IP アドレスマッピング)。|
|logonType|logonType|ユーザーのサインイン方法。 使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|String|ユーザーの Active Directory (社内) セキュリティ識別子 (SID)。|
|riskScore|String|ユーザーアカウントのプロバイダーが生成/計算したリスクスコア。 推奨値の範囲0-1。パーセンテージに相当します。|
|userAccountType|userAccountSecurityType|ユーザーアカウントの種類 (グループメンバーシップ) (Windows 定義あたり)。 使用可能な値は、`unknown`、`standard`、`power`、`administrator` です。|
|userPrincipalName|String|ユーザーのサインイン名-インターネット形式: (ユーザーアカウント名) @ (ユーザーアカウントの DNS ドメイン名)。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
