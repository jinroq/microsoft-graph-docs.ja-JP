---
title: educationFileResource リソースの種類
description: 送信または割り当てに関連付けられているファイル オブジェクトを表す educationResource のサブクラスです。  この例では、ファイルは特別なファイル (Word、Excel、およびなど) のいずれかがファイル システム内で特別な処理がないです。 このリソースに接続されている送信または割り当てに関連付けられている**resourceFolder**では、ファイル リソースを格納してください。
ms.openlocfilehash: b3ba77b6b9243d987ad1137afe6d2206e47dadaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070551"
---
# <a name="educationfileresource-resource-type"></a>educationFileResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

送信または割り当てに関連付けられているファイル オブジェクトを表す[educationResource](educationresource.md)のサブクラスです。  この例では、ファイルは特別なファイル (Word、Excel、およびなど) のいずれかがファイル システム内で特別な処理がないです。 このリソースに接続されている送信または割り当てに関連付けられている**resourceFolder**では、ファイル リソースを格納してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fileUrl|String|ファイル リソースのディスク上の場所です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->