---
title: usersecuritystate リソースの種類
description: ユーザーアカウントに関するステートフルな情報を含みます。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f451f2bc42500eee15bd59809c124a79186916f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463811"
---
# <a name="usersecuritystate-resource-type"></a>usersecuritystate リソースの種類

ユーザーアカウントに関するステートフルな情報を含みます。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|usersecuritystate|String|AAD user オブジェクト識別子 (GUID)-物理/マルチアカウントユーザーエンティティを表します。|
|アカウント|String|ユーザーアカウントのアカウント名 (Active Directory ドメインまたは DNS ドメインなし)-(と`mailNickName`も呼ばれます)。|
|domainName|String|ユーザーアカウントの NetBIOS/Active Directory ドメイン (つまり、"ドメイン \ ユーザー名" の形式)。|
|emailRole|emailRole|電子メール関連の警告の場合-ユーザーアカウントの電子メール ' ロール '。 使用可能な値は、`unknown`、`sender`、`recipient` です。|
|isvpn|Boolean|ユーザーが VPN を介してログオンしたかどうかを示します。|
|logondatetime|DateTimeOffset|サインインが発生した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|logonId|String|ユーザーのサインイン ID。|
|logonIp|String|サインイン要求の送信元の IP アドレス。|
|logonlocation|String|このユーザーによってユーザーのサインインイベントに関連付けられている場所 (IP アドレスマッピング)。|
|logonType|logonType|ユーザーのサインイン方法。 可能な値は `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service` です。|
|onPremisesSecurityIdentifier|String|ユーザーの Active Directory (社内) セキュリティ識別子 (SID)。|
|riskScore|String|ユーザーアカウントのプロバイダーが生成/計算したリスクスコア。 推奨値の範囲0-1。パーセンテージに相当します。|
|userAccountType|userAccountSecurityType|ユーザーアカウントの種類 (グループメンバーシップ) (Windows 定義あたり)。 可能な値は、`unknown`、`standard`、`power`、`administrator` です。|
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
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
