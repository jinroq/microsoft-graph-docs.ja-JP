---
title: プラン/プラン contextのコレクションリソースの種類
description: " 値は、\"plan/コンテキスト詳細\" オブジェクトです。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 2e2f292de763674510f6da5a8aad90fe8e17ab7f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344400"
---
# <a name="plannerplancontextdetailscollection-resource-type"></a>プラン/プラン contextのコレクションリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


plan**グループ**は、プランがリンクされている外部コンテキストのコレクションを表します。 このリソースは、オープンタイプであり、" [plan" プランの詳細](plannerplandetails.md)オブジェクトの一部です。 プロパティと値のペアのプロパティ名は、コンテキストのアプリケーション固有の識別子です。値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトです。


## <a name="properties"></a>プロパティ
オープン型のプロパティは、クライアントで定義できます。 この場合、クライアントは、プロパティ名として、外部コンテキストを表すディスティンクティブ識別子を使用する必要があります。 プロパティの値は、" [plan/コンテキスト詳細](plannerplancontextdetails.md)" オブジェクトである必要があります。 OData に基づいて、オープン型のプロパティ名に次の文字を`.`含める`:`こと`@`は`%`できません:、、、。 これらの文字は、URL エンコード形式でエンコードする必要があります。 [お気に入り] の一覧から項目を削除するには、その値を[プラン](plannerplancontextcollection.md)から削除する必要があります。このコレクションは、このオブジェクトのエントリを自動的に削除します。

## <a name="json-representation"></a>JSON 表記
リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
}-->

```json
{
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerPlanContextDetailsCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
