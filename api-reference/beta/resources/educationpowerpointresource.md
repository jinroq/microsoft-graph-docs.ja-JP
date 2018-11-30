---
title: educationPowerPointResource リソースの種類
description: 'EducationResource のサブクラスです。 これは、PowerPoint のリソースです。 関連付けられている**fileResource**ディレクトリに、PowerPoint ファイルをアップロードする必要があります、 '
ms.openlocfilehash: a83a78449ecb7c64f62557ddfa642ab02b55c206
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071875"
---
# <a name="educationpowerpointresource-resource-type"></a>educationPowerPointResource リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[EducationResource](educationresource.md)のサブクラスです。 これは、PowerPoint のリソースです。 送信または割り当てに関連付けられている**fileResource**ディレクトリには、PowerPoint ファイルをアップロードする必要があります。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|fileUrl|String|ディスク上のファイルの場所です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->