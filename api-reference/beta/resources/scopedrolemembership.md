---
title: scopedRoleMembership リソースの種類
description: スコープ指定された役割メンバーシップは、管理単位 (AU) に対してさらにスコープを設定する、ディレクトリロールのユーザーのメンバーシップを記述します。  これにより、テナント全体の会社 adminsistrator が、組織のサブセット (AU で定義されているサブセット) 内のユーザーとグループを管理するための管理者権限を委任できるようになります。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2580555bf3d10454aad9052f694ff1a62bf4b9b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965286"
---
# <a name="scopedrolemembership-resource-type"></a>scopedRoleMembership リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

スコープ指定された役割メンバーシップは、管理単位 (AU) に対してさらにスコープを設定する、ディレクトリロールのユーザーのメンバーシップを記述します。  これにより、テナント全体の会社 adminsistrator が、組織のサブセット (AU で定義されているサブセット) 内のユーザーとグループを管理するための管理者権限を委任できるようになります。

## <a name="methods"></a>メソッド
このリソースへの直接クエリはサポートされていません。  スコープ指定された役割のメンバーシップのクエリを実行する方法、およびスコープ付きの役割メンバーシップを追加および削除する方法については、「操作の[単位](administrativeunit.md)」を参照してください。 

## <a name="properties"></a>プロパティ
| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
|administrativeUnitId|string|ディレクトリの役割のスコープが設定されている管理単位の一意の識別子|
|id|string| スコープ指定された役割のメンバーシップの一意識別子。 読み取り専用です。|
|roleId|string| メンバーが属しているディレクトリロールの一意の識別子。|
|roleMemberInfo|[identity](identity.md)| 役割メンバーの id 情報。 このスコープ指定された役割のメンバーであるユーザーを表します。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
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
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
