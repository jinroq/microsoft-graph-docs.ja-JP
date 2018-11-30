---
title: エンティティ リソースの種類
description: 別のアプリケーションを呼び出すクライアント アプリケーションを要求することがまたは指定したアプリケーションのロールのユーザーまたはグループにアプリケーションを割り当てるに使用でき、アプリケーション ロールを表します。 ServicePrincipal エンティティおよびアプリケーション エンティティの**appRoles**プロパティは、**エンティティ**のコレクションです。
ms.openlocfilehash: f87ef6f40fbeb18ec4b3a2373fb2a19e14da84a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067923"
---
# <a name="approle-resource-type"></a>エンティティ リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

別のアプリケーションを呼び出すクライアント アプリケーションを要求することがまたは指定したアプリケーションのロールのユーザーまたはグループにアプリケーションを割り当てるに使用でき、アプリケーション ロールを表します。 [ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**appRoles**プロパティは、**エンティティ**のコレクションです。

> 重要: この機能は現在のリリースでは無効です。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
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
|allowedMemberTypes|String コレクション|設定「アプリケーション」、またはその両方を設定を [ユーザー]、またはその他のアプリケーション (デーモン サービスのシナリオでは、このアプリケーションにアクセスしている) に、このアプリケーションの役割の定義ユーザーおよびグループに割り当てることができるかどうかを指定します。|
|説明|String|アクセス許可は、ヘルプ テキストの割り当ての管理アプリケーションで表示されると、経験に同意するものです。|
|displayName|String|管理者同意し、アプリケーションの割り当ての経験で表示されるアクセス許可の名前を表示します。|
|ID|Guid|**AppRoles**コレクション内のロールの一意の識別子です。|
|isEnabled|Boolean|作成するか、役割の定義の更新、これを**true** (既定値) に設定しなければなりません。 ロールを削除するには、この必要があります最初設定**false を指定**します。  その時点で、後続の呼び出しでこのロールが削除されます。|
|value|文字列|認証とアクセス トークンでは、アプリケーションが期待する役割要求の値を指定します。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->