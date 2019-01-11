---
title: agreementFileData リソースの種類
description: Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。
localization_priority: Normal
ms.openlocfilehash: 64de3a72ad648225f24429987f5729f76ed8a2e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815219"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。

## <a name="properties"></a>プロパティ
| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|data|Binary|PDF 文書の使用の条件を表すデータです。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
