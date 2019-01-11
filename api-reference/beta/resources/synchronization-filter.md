---
title: リソースの種類のフィルター
description: アプリケーション オブジェクトを準備する必要がありますを決定します。 たとえば、米国内にあるユーザーのみを提供する可能性があります。 スコープ フィルターが存在する場合、フィルターを満たしていないオブジェクトは同期中にスキップされます。
localization_priority: Normal
ms.openlocfilehash: 754271e9d33159a14d1abf356280dd619643002f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894412"
---
# <a name="filter-resource-type"></a>リソースの種類のフィルター

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーション オブジェクトを準備する必要がありますを決定します。 たとえば、米国内にあるユーザーのみを提供する可能性があります。 スコープ フィルターが存在する場合、フィルターを満たしていないオブジェクトは同期中にスキップされます。

フィルターは、[オブジェクトのマッピング](synchronization-objectmapping.md)の一部です。 フィルターのグループのいくつかのセットで構成されていて、各フィルター グループが 1 つまたは複数の句を保持します。 オブジェクトは、グループのスコープ内と見なされます (グループが評価され、 `true`) にグループのすべての句が評価される場合にのみ`true`。

オブジェクトは、グループのスコープ内と見なされます (グループのセットが評価され、 `true`) 場合は、セット内のグループのいずれかが評価され、 `true`。

詳細については、[属性ベースのアプリケーションのスコープ フィルターを使用してプロビジョニング](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-scoping-filters)を参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|categoryFilterGroups|[filterGroup](synchronization-filtergroup.md)コレクション|`*Experimental*`かどうか特定のオブジェクトが所属するグループのセットをフィルター処理し、このオブジェクトのマッピングの一部として処理する必要があります。 オブジェクトがスコープ内と見なされる*場合は、コレクション内のグループのいずれかが評価され、 `true` *。|
|グループ|[filterGroup](synchronization-filtergroup.md)コレクション|プロビジョニング用のスコープ、オブジェクトが指定されているかどうかを決定するために使用するグループ セットをフィルター処理します。 **これは、ほとんどの場合に使用するフィルター**です。 そのフィルターではありませんので、特定の時点でこのフィルターを満たすために使用されるオブジェクトと、オブジェクトまたはフィルターが変更された場合はそのようなオブジェクトで満足できなくなった場合、* はプロビジョニング解除」します。 オブジェクトがスコープ内と見なされる*場合は、コレクション内のグループのいずれかが評価され、 `true` *。|
|inputFilterGroups|[filterGroup](synchronization-filtergroup.md)コレクション|`*Experimental*`グループ セットのオブジェクトをディレクトリから読み取ることの初期の段階でフィルターをかけるためにフィルターを適用します。 オブジェクトは、このフィルターを満たしていない場合にする処理は行われません。 重要満たされる場合、オブジェクトは、特定の時点でこのフィルターを満たすために使用し、オブジェクト、またはフィルターが変更されていてそのフィルターはないことを理解するのなどのオブジェクト*が取得するが準備されていません*。 オブジェクトがスコープ内と見なされる*場合は、コレクション内のグループのいずれかが評価され、 `true` *。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
