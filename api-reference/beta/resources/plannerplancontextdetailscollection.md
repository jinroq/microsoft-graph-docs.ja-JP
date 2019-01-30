---
title: plannerPlanContextDetailsCollection リソースの種類
description: " 値は、plannerPlanContextDetails オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642941"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>plannerPlanContextDetailsCollection リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


**PlannerPlanContextDetailsCollection**リソースでは、プランがリンクされている外部のコンテキストのコレクションを表します。 このリソースは、オープン型であり、 [plannerPlanDetails](plannerplandetails.md)オブジェクトの一部であります。 プロパティ名、プロパティ値のペアでは、アプリケーション固有のコンテキストの識別子値は、 [plannerPlanContextDetails](plannerplancontextdetails.md)オブジェクトです。


## <a name="properties"></a>プロパティ
クライアントでは、オープン型のプロパティを定義できます。 この場合、クライアントは、プロパティ名と外部のコンテキストを表す特徴的な識別子を使用する必要があります。 プロパティの値は、 [plannerPlanContextDetails](plannerplancontextdetails.md)オブジェクトである必要があります。 OData を基に、オープン型のプロパティ名は次の文字を含めることはできません: `.`、 `:`、 `@`、 `%`。 これらの文字は、URL エンコード形式にエンコードする必要があります。 お気に入りの一覧で項目を削除するに値が必要な[plannerPlanContextCollection](plannerplancontextcollection.md)コレクションから削除する代わりに、このオブジェクトのエントリを自動的に削除されます。


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerplancontextdetailscollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
