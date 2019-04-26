---
title: プラン/プラン contextのコレクションリソースの種類
description: " 値は、\"plan/コンテキスト詳細\" オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: ca1625a4bf137fc14cc780df4d4d1e5ec3bb226e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571858"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>プラン/プラン contextのコレクションリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


plan**グループ**は、プランがリンクされている外部コンテキストのコレクションを表します。 このリソースは、オープンタイプであり、" [plan" プランの詳細](plannerplandetails.md)オブジェクトの一部です。 プロパティと値のペアのプロパティ名は、コンテキストのアプリケーション固有の識別子です。値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトです。


## <a name="properties"></a>プロパティ
オープン型のプロパティは、クライアントで定義できます。 この場合、クライアントは、プロパティ名として、外部コンテキストを表すディスティンクティブ識別子を使用する必要があります。 プロパティの値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトである必要があります。 OData に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`@`は`%`できません:、、、。 これらの文字は、URL エンコード形式でエンコードする必要があります。 [お気に入り] の一覧から項目を削除するには、その値を[プラン](plannerplancontextcollection.md)から削除する必要があります。このコレクションは、このオブジェクトのエントリを自動的に削除します。


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
