---
title: governanceRoleAssignment リソースの種類
description: ロールにユーザーまたはグループの割り当てを表します。
localization_priority: Normal
ms.openlocfilehash: d873b122f319ca82882727f065818b33f7f9d44d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882692"
---
# <a name="governanceroleassignment-resource-type"></a>governanceRoleAssignment リソースの種類
> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ロールにユーザーまたはグループの割り当てを表します。

特権を持つユーザーの管理 (PIM) には、割り当ての 2 つの種類がサポートされています。

1. アクティブな割り当てでは、リソースに対してダイレクト/有効化済アクセスを表します。
2. 対象となる割り当てのないアクセスと直接アクセスの間でのリソースへのアクセス権限の中間の段階を表します。 管理者はユーザーまたはグループに割り当てることができます`eligible assignment`アクセス権が必要な事前に、必ず`activation`に、`eligible assignment`は、いくつかの時間のリソースへのインスタント アクセスを得るために必要な。 ライセンス認証の後、`active assignment`のアクティブ化の状態を示すためにユーザーまたはグループのメンバーが作成されます。

## <a name="methods"></a>メソッド

| メソッド          | 戻り値の型 |説明|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |ロール割り当てのエンティティのプロパティと関係を参照してください。|
|[List](../api/governanceroleassignment-list.md) | [governanceRoleAssignment](../resources/governanceroleassignment.md)コレクション|リソースの役割の割り当ての一覧を表示します。 |
|[Export](../api/governanceroleassignment-export.md) | オクテット ストリーム |リソースの役割の割り当てのコレクションをダウンロードし、名前を付けて、`.csv`ファイルです。|

No `POST`、 `PUT`、 `PATCH`、または`DELETE`の操作はサポートされて、`roleAssignments`のエンティティ セット。 任意の作成では、更新、および削除の操作で`governanceRoleAssignment`で行われます`governanceRoleAssignmentRequest`。

## <a name="properties"></a>プロパティ
| プロパティ  | 種類      |説明|
|:----------|:----------|:----------|
|ID         |String     |役割の割り当ての ID です。 GUID 形式であります。|
|resourceId |String     |必須。 ロールの割り当てに関連付けられているリソースの ID です。 |
|roleDefinitionId|String|必須。 ロールの割り当てに関連付けられている役割の定義の ID です。 |
|subjectId|String       |必須。 ロールの割り当てに関連付けられているサブジェクトの ID です。 |
|linkedEligibleRoleAssignmentId|String|場合は、`active assignment`のアクティブ化のために作成されると、 `eligible assignment`、その ID を表す`eligible assignment`です。値は、それ以外の場合、 `null`。 |
|externalId   |String     |外部 ID プロバイダーの役割の割り当てを識別するために使用されるリソースです。|
|startDateTime|DateTimeOffset|役割の割り当ての開始時刻。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|非永続的なロールの割り当てでは、これは、時間とロールの割り当て、期限切れにします。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|assignmentState|String  |割り当ての状態です。 値は、します。 <ul><li> `Eligible`対象となる割り当ての</li><li> `Active`-直接割り当てられている場合`Active`管理者、またはユーザーが対象となる割り当ての有効化します。</li></ul>|
|memberType|String      |メンバーの型。 値を指定できます。 <ul><li>`Inherited`ロールの割り当ては、親のリソースのスコープから継承します。</li><li>`Group`ロールの割り当ては継承されませんが、グループの割り当てのメンバーシップは、</li><li>`User`-ロールの割り当ては、どちらも継承も割り当てをグループ化します。</li></ul>|


## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|リソース|[governanceResource](../resources/governanceresource.md)|読み取り専用です。 ロールの割り当てに関連付けられているリソースです。 |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|読み取り専用です。 ロールの割り当てに関連付けられているロールの定義。 |
|subject|[governanceSubject](../resources/governancesubject.md)|読み取り専用です。 ロールの割り当てに関連付けられている件名です。 |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|読み取り専用です。 場合は、`active assignment`のアクティブ化のために作成されると、 `eligible assignment`、そのオブジェクトを表す`eligible assignment`です。値は、それ以外の場合、 `null`。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。


<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
