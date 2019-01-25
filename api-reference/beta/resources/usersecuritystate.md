---
title: userSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 62a54a996d7fe9c892da797cee352a57d0782035
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517240"
---
# <a name="usersecuritystate-resource-type"></a>userSecurityState リソースの種類

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザー アカウントに関するステートフルな情報が含まれています。

## <a name="properties"></a>プロパティ

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|aadUserId|String|AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。|
|accountName|String|(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる`mailNickName`)。|
|domainName|String|ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。|
|emailRole|emailRole|電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。 可能な値は、`unknown`、`sender`、`recipient` です。|
|isVpn|ブール値|VPN 経由でユーザーをログオンするかどうかを示します。|
|logonDateTime|DateTimeOffset|サインインが発生した時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。|
|logonId|String|ユーザーのサインイン ID|
|logonIp|String|IP アドレスは、サインイン要求が出されたからです。|
|logonLocation|String|(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。|
|logonType|logonType|ユーザーのサインインの方法です。 使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。|
|onPremisesSecurityIdentifier|String|アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。|
|riskScore|String|ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。 0 - 1 パーセントに相当する値の範囲をお勧めします。|
|userAccountType|userAccountSecurityType|ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。 可能な値は、`unknown`、`standard`、`power`、`administrator` です。|
|userPrincipalName|文字列|ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/usersecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
