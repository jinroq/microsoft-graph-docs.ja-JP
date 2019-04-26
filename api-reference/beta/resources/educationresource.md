---
title: educationResource リソースの種類
description: システム内のすべてのリソースオブジェクトのスーパークラス。 リソースが**割り当て**または**送信**(またはその両方) に関連付けられています。これは、指定された学習オブジェクトを表します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0713b6cb00e0b5e0b1e33181b43691b1d5b6530d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340524"
---
# <a name="educationresource-resource-type"></a>educationResource リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

システム内のすべてのリソースオブジェクトのスーパークラス。 リソースが**割り当て**または**送信**に関連付けられています。これは、渡される、または渡される learning オブジェクトを表します。 リソースを直接インスタンス化することはできません。使用されているリソースの種類を表すサブクラスを作成する必要があります。

このリソースは、すべてのリソースの種類で共通のプロパティを格納します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|リソースの作成者。|
|createdDateTime|リソースが作成された時点の時間。  DateTimeOffset|Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|displayName|String|リソースの表示名。|
|lastModifiedBy|[identitySet](identityset.md)|リソースを最後に変更したユーザー。|
|lastModifiedDateTime|DateTimeOffset|リソースが最後に変更された時点の時刻。  Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
