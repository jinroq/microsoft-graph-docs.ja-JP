---
title: educationAssignmentResource リソースの種類
description: 割り当てに関連付けられているリソースを格納するラッパー オブジェクトを返します。 ラッパーが**distributeForStudentWork**プロパティを追加し、このリソースが、あることを示します
ms.openlocfilehash: 6907af5e4408248487b118c390bb2ec209700124
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070558"
---
# <a name="educationassignmentresource-resource-type"></a>educationAssignmentResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

割り当てに関連付けられているリソースを格納するラッパー オブジェクトを返します。 ラッパーは、 **distributeForStudentWork**プロパティを追加し、このリソースを受講者の提出書類にコピーされることを示します。  オブジェクトはコピーされませんが、各受講者は、割り当てのリソースへのリンクが表示されます。 受講者はこのリソースを更新できません。 これは、受講者に次ことが何もに、先生からの配布資料です。 リソースが分散している場合は、各受講者がリソースの一覧で、データを送信このリソースのコピーが表示されます。 各受講者はそのコピーを変更し、グレーディングのために送信することになります。


## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[EducationAssignmentResource を取得します。](../api/educationassignmentresource-get.md) | [educationAssignmentResource](educationassignmentresource.md) |**EducationAssignmentResource**オブジェクトのプロパティと関係を参照してください。|
|[Update](../api/educationassignmentresource-update.md) | [educationAssignmentResource](educationassignmentresource.md) |**EducationAssignmentResource**オブジェクトを更新します。 |
|[削除](../api/educationassignmentresource-delete.md) | なし |**EducationAssignmentResource**オブジェクトを削除します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|distributeForStudentWork|ブール値|受講生受講者の変更、および送信のため送信するたびにこのリソースをコピーするかどうかを示します。|
|id|String| このリソースの ID です。 読み取り専用。|
|resource|[educationResource](educationresource.md)|リソースがこの割り当てに関連付けられているオブジェクト。|

## <a name="relationships"></a>リレーションシップ
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
