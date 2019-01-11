---
title: agreementAcceptance リソースの種類
description: Azure Active Directory (Azure AD) の電源を使用して会社のカスタマイズ可能な条件の範囲内のユーザーの現在の状態を表します。
localization_priority: Normal
ms.openlocfilehash: b1c8a5e40fe6a12daf23566ae902ddf61f3ee4df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828284"
---
# <a name="agreementacceptance-resource-type"></a>agreementAcceptance リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory (Azure AD) の電源を使用して会社のカスタマイズ可能な条件の範囲内のユーザーの現在の状態を表します。

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a>プロパティ
| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
|agreementFileId|String|ユーザーによって承諾される契約書のファイルの ID です。|
|agreementId|String|契約の ID です。|
|id|String| 読み取り専用です。|
|recordedDateTime|DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|state|文字列| 使用可能な値は、`accepted`、`declined` です。|
|userDisplayName|String|受け入れの記録時に、ユーザーの名前を表示します。|
|userEmail|String|受け入れが記録された場合のユーザーの電子メール。|
|userId|String|契約を承諾したユーザーの ID です。|
|userPrincipalName|String|受け入れが記録された場合のユーザーの UPN。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
