---
title: agreementFileData リソースの種類
description: Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。
ms.openlocfilehash: 557725e14f4954f8b2c10112e1013beb71dda0be
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070398"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory の blob ファイルの使用許諾契約書の条項を (Azure AD) を表します。

## <a name="properties"></a>プロパティ
| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|data|バイナリ|PDF 文書の使用の条件を表すデータです。 読み取り専用。|

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
