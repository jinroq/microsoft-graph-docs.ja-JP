---
title: directoryObjectPartnerReference リソースの種類
description: パートナー テナント内のディレクトリ オブジェクトへの参照を表します。 directoryObject から継承します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 17bab72fad3e03b843975ae62261fac9c09af791
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918540"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryObjectPartnerReference リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

パートナー組織内のディレクトリ オブジェクトへの参照を表します。 [directoryObject](directoryobject.md?view=graph-rest-beta) から継承します。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|説明|String| オブジェクトの説明が返されます。 読み取り専用です。 |
|displayName|String| グループまたはアプリケーションのように、返されるディレクトリ オブジェクトの名前です。 読み取り専用です。 |
|externalPartnerTenantId|Guid| パートナー テナントにテナントの識別子です。 読み取り専用です。 |
|id|String| リソースの一意識別子。 [directoryObject](directoryobject.md?view=graph-rest-beta) から継承されます。 読み取り専用です。 |
|objectType|String| パートナー テナントで参照されるオブジェクトの型。 読み取り専用です。 |

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
<!-- {
  "type": "#page.annotation",
  "description": "directoryObjectPartnerReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
