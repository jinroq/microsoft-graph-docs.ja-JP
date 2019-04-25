---
title: filter リソースの種類
description: アプリケーションにどのオブジェクトをプロビジョニングするかを指定します。 たとえば、US にあるユーザーのみをプロビジョニングする場合があります。 スコープフィルターが指定されている場合、フィルターを満たしていないオブジェクトは、同期中にスキップされます。
localization_priority: Normal
ms.openlocfilehash: acc9f2efcfeef68ee3beda7dc720b5da5dea2b1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582117"
---
# <a name="filter-resource-type"></a>filter リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

アプリケーションにどのオブジェクトをプロビジョニングするかを指定します。 たとえば、US にあるユーザーのみをプロビジョニングする場合があります。 スコープフィルターが指定されている場合、フィルターを満たしていないオブジェクトは、同期中にスキップされます。

フィルターは、[オブジェクトマッピング](synchronization-objectmapping.md)の一部です。 フィルターグループの複数のセットで構成され、各フィルターグループは1つまたは複数の句を保持します。 グループのすべての句が評価される場合にのみ、グループの`true`スコープ内でオブジェクトが考慮され`true`ます (グループは評価されます)。

セット内のいずれかのグループがに`true` `true`評価される場合、グループセットのスコープ内でオブジェクトが考慮されます (グループセットはに評価されます)。

詳細については、「[スコープフィルターを使用した属性ベースのアプリケーションのプロビジョニング](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)」を参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|カテゴリの filtergroups|[filtergroup](synchronization-filtergroup.md)コレクション|`*Experimental*`指定したオブジェクトが属しているかどうかを判断し、このオブジェクトマッピングの一部として処理する必要があることを決定するために使用されるフィルタグループセット。 *コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。|
|groups|[filtergroup](synchronization-filtergroup.md)コレクション|フィルターグループセットは、指定されたオブジェクトがプロビジョニングの対象になっているかどうかを判断するために使用されます。 **このフィルターは、ほとんどの場合に使用する必要があり**ます。 オブジェクトが指定された時点でこのフィルターに適合し、フィルターの条件が満たされなくなるようにオブジェクトまたはフィルターが変更された場合は、そのようなオブジェクト * はプロビジョニング解除されます。 *コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。|
|inputfiltergroups|[filtergroup](synchronization-filtergroup.md)コレクション|`*Experimental*`フィルタグループセットは、ディレクトリからの読み取りの初期段階でオブジェクトをフィルター処理するために使用されます。 オブジェクトがこのフィルターを満たしていない場合は、それ以上処理されません。 理解しておく必要がある重要な点は、オブジェクトが指定された時点でこのフィルターを満たしている場合に、フィルターが満たされなくなるようにオブジェクトまたはフィルターが変更された場合、そのようなオブジェクト*はプロビジョニング解除されません*。 *コレクション内のいずれかのグループがに`true`評価される場合*、オブジェクトはスコープ内で考慮されます。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filter"
}-->

```json
{
  "categoryFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "groups": [{"@odata.type": "microsoft.graph.filterGroup"}],
  "inputFilterGroups": [{"@odata.type": "microsoft.graph.filterGroup"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
