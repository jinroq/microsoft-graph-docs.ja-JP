---
title: userSecurityState リソースの種類
description: ユーザー アカウントに関するステートフルな情報が含まれています。
ms.openlocfilehash: dbb4b6600cc11a75c84f2f0b233535d012309f88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022738"
---
# <a name="usersecuritystate-resource-type"></a>userSecurityState リソースの種類

ユーザー アカウントに関するステートフルな情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|aadUserId|String|AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。|
|accountName|String|(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる`mailNickName`)。|
|domainName|String|ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。|
|emailRole|emailRole|電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。 可能な値は、`unknown`、`sender`、`recipient` です。|
|isVpn|ブール値|VPN 経由でユーザーをログオンするかどうかを示します。|
|logonDateTime|DateTimeOffset|サインインが発生した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|logonId|String|ユーザーのサインイン ID|
|logonIp|String|IP アドレスは、サインイン要求が出されたからです。|
|logonLocation|String|(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。|
|logonType|logonType|ユーザーのサインインの方法です。 使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|String|アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。|
|riskScore|String|ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。 0 - 1 パーセントに相当する値の範囲をお勧めします。|
|userAccountType|userAccountSecurityType|ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。 可能な値は、`unknown`、`standard`、`power`、`administrator` です。|
|userPrincipalName|String|ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。|

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
