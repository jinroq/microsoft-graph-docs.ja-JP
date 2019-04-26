---
title: directoryobjectpartnerreference リソースの種類
description: パートナーテナント内のディレクトリオブジェクトへの参照を表します。 directoryObject から継承します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 91d33993ea83ea7eba883534efb513fa80287a64
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340852"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryobjectpartnerreference リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

パートナー組織内のディレクトリオブジェクトへの参照を表します。 [directoryObject](directoryobject.md) から継承します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|description|String| 返されるオブジェクトの説明。 読み取り専用です。 |
|displayName|String| グループまたはアプリケーションなど、返されるディレクトリオブジェクトの名前。 読み取り専用です。 |
|externalpartnertenantid|Guid| パートナーテナントのテナント識別子。 読み取り専用。 |
|id|String| リソースの一意識別子。 [directoryObject](directoryobject.md) から継承されます。 読み取り専用です。 |
|objectType|文字列| パートナーテナント内の参照されるオブジェクトの種類。 読み取り専用です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryObjectPartnerReference"
}-->

```json
{
  "description": "string ",
  "displayName": "string",
  "externalPartnerTenantId": "string (identifier)",
  "id": "string (identifier)",
  "objectType": "string"
}
```

## <a name="see-also"></a>関連項目

- [ID のリストからディレクトリ オブジェクトを取得します。](/graph/api/directoryobject-getbyids?view=graph-rest-beta)

<!-- uuid: fbec8cd7-cfe4-431d-87fc-d102cd2841a4
2018-12-06 02:01:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
