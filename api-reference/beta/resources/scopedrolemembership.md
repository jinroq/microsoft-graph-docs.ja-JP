---
title: scopedRoleMembership リソースの種類
description: スコープ ロール メンバーシップでは、スコープ管理単位 (AU) には、さらに、ディレクトリのロールのユーザーのメンバーシップについて説明します。  これは、ユーザーおよび組織の一部のグループ (、AU で定義されるサブセット) を管理するユーザーに管理者特権を委任するテナント規模の企業の adminsistrator を許可するためのメカニズムを提供します。
ms.openlocfilehash: bd635a5b1b06b98657ba24c397e2f67afb76fa8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069796"
---
# <a name="scopedrolemembership-resource-type"></a>scopedRoleMembership リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

スコープ ロール メンバーシップでは、スコープ管理単位 (AU) には、さらに、ディレクトリのロールのユーザーのメンバーシップについて説明します。  これは、ユーザーおよび組織の一部のグループ (、AU で定義されるサブセット) を管理するユーザーに管理者特権を委任するテナント規模の企業の adminsistrator を許可するためのメカニズムを提供します。

## <a name="methods"></a>メソッド
このリソースへの直接のクエリはサポートされていません。  スコープ ロール メンバーシップの追加と削除と同様にスコープ ロールのメンバーシップを照会する方法についての情報を表示する[単位数の管理](administrativeunit.md)トピックを参照してください。 

## <a name="properties"></a>プロパティ
| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
|administrativeUnitId|文字列|ディレクトリの役割のスコープは、管理単位の一意の識別子|
|ID|文字列| スコープ ロール メンバーシップの一意の識別子です。 読み取り専用。|
|roleId|文字列| メンバーが含まれるディレクトリの役割の一意の識別子です。|
|roleMemberInfo|[identity](identity.md)| ロール メンバーの識別情報です。 このスコープの役割のメンバーであるユーザーを表します。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->