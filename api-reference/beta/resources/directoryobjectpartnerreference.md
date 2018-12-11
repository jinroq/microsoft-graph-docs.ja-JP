---
title: directoryObjectPartnerReference リソースの種類
description: パートナー テナント内のディレクトリ オブジェクトへの参照を表します。 directoryObject から継承します。
ms.openlocfilehash: ebdd7380eaa6b59488aca46120339f7175b640fa
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27224128"
---
# <a name="directoryobjectpartnerreference-resource-type"></a>directoryObjectPartnerReference リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

パートナー組織内のディレクトリ オブジェクトへの参照を表します。 [directoryObject](directoryobject.md?view=graph-rest-beta) から継承します。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|説明|String| オブジェクトの説明が返されます。 読み取り専用です。 |
|displayName|String| グループまたはアプリケーションのように、返されるディレクトリ オブジェクトの名前です。 取得のみ可能な値です。 |
|externalPartnerTenantId|Guid| パートナー テナントにテナントの識別子です。 読み取り専用。 |
|id|String| リソースの一意識別子。 [directoryObject](directoryobject.md?view=graph-rest-beta) から継承されます。 取得のみ可能な値です。 |
|objectType|String| パートナー テナントで参照されるオブジェクトの型。 取得のみ可能な値です。 |

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
