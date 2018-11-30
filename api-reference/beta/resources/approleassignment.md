---
title: appRoleAssignment リソースの種類
description: ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。 この例では、ロールの割り当てと、アプリケーション タイルは、ユーザーのアプリケーションのアクセス パネルを表示します。 このエンティティは、特定のロールで、リソース アプリケーションに別の (サービスの主体としてモデル化された) アプリケーションのアクセス権を付与するも使用できます。 ことができます作成、読み取り、更新、およびロールの割り当てを削除します。
ms.openlocfilehash: 97155bde12735ebd8a7674e0dbf20dae30e53f14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067936"
---
# <a name="approleassignment-resource-type"></a>appRoleAssignment リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ユーザーまたはグループがアプリケーションに割り当てられるときの記録に使用します。 この例では、ロールの割り当てと、アプリケーション タイルは、ユーザーのアプリケーションのアクセス パネルを表示します。 このエンティティは、特定のロールで、リソース アプリケーションに別の (サービスの主体としてモデル化された) アプリケーションのアクセス権を付与するも使用できます。 ことができます作成、読み取り、更新、およびロールの割り当てを削除します。


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approleassignment"
}-->

```json
{
  "creationTimestamp": "String (timestamp)",
  "id": "guid (identifier)",
  "principalDisplayName": "string",
  "principalId": "guid",
  "principalType": "string",
  "resourceDisplayName": "string",
  "resourceId": "guid"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|creationTimestamp|DateTimeOffset|交付が作成された時刻。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|ID|Guid|プリンシパルに割り当てられたロールの id です。  この役割は、 **appRoles**プロパティにターゲットのリソース アプリケーション**引数 resourceId**で宣言されなければなりません。 リソースですべてのアクセス許可が宣言されていない場合は、デフォルトの id (GUID は 0) を指定してください。 キー。 null 許容ではありません。 |
|principalDisplayName|String|アクセス権を与えられたプリンシパルの表示名。|
|principalId|Guid|アクセスを付与されているプリンシパルの一意の識別子 (**id**) です。 必要なを作成します。            |
|principalType|String|プリンシパルの種類。  「ユーザー」、「グループ」または"ServicePrincipal"指定できます。|
|resourceDisplayName|String|割り当てが作成するリソースの表示名。|
|resourceId|Guid|割り当てが作成する対象のリソース (サービス主体) の一意の識別子 (**id**) です。|

## <a name="relationships"></a>リレーションシップ
なし


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[AppRoleAssignment を取得します。](../api/approleassignment-get.md) | [appRoleAssignment](approleassignment.md) |AppRoleAssignment オブジェクトのプロパティと関係を参照してください。|
|[Update](../api/approleassignment-update.md) | [appRoleAssignment](approleassignment.md)   |AppRoleAssignment オブジェクトを更新します。 |
|[削除](../api/approleassignment-delete.md) | なし |AppRoleAssignment オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->