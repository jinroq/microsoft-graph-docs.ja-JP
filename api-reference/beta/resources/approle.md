---
title: appRole リソースの種類
description: 別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。 ServicePrincipal エンティティおよび application エンティティの**approles**プロパティは、 **approles**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 35c26e52c5d7eb9529474d08a43b68fceddfc954
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013327"
---
# <a name="approle-resource-type"></a>appRole リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

別のアプリケーションを呼び出しているクライアントアプリケーションによって要求されるか、または指定されたアプリケーションロールのユーザーまたはグループにアプリケーションを割り当てるために使用される可能性があるアプリケーションロールを表します。 [Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**Approles**プロパティは、 **approles**のコレクションです。

> 重要: この機能は現在のリリースでは無効になっています。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|allowedMemberTypes|文字列コレクション|"Application" に設定するか、またはその両方に設定して、このアプリの役割定義をユーザーとグループに割り当てることができるようにするかどうかを指定します。 "User" に設定するか、または (デーモンサービスシナリオでこのアプリケーションにアクセスしている) 他のアプリケーションに割り当てます。|
|description|String|管理者アプリの割り当てと同意エクスペリエンスに表示されるアクセス許可ヘルプテキスト。|
|displayName|String|管理者の同意とアプリの割り当てエクスペリエンスに表示されるアクセス許可の表示名。|
|id|Guid|Approles コレクション内の**** 一意のロール識別子。 新しいアプリの役割を作成する場合は、新しい Guid 識別子を指定する必要があります。 |
|isEnabled|Boolean|アプリの役割を作成または更新する場合は、 **true** (既定値) に設定する必要があります。 役割を削除するには、最初に**false**に設定する必要があります。  その時点で、以降の呼び出しでは、この役割が削除される可能性があります。|
|戻す|String| 読み取り専用です。 アプリケーションオブジェクトまたは ServicePrincipal オブジェクトでアプリの役割が定義されているかどうかを指定します。 POST または PATCH 要求に含まれていてはなり_ません_。 |
|value|文字列|認証とアクセストークンで`roles`クレームに含める値を指定します。 長さが120文字を超えることはできません。 許可される`:` `!` `#` `$` `%`文字`&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `0-9`内`A-Z`の文字、 `a-z`および。 `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` スペース文字を含むその他の文字は使用できません。  |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
