---
title: educationIdentityMatchingConfiguration リソースの種類
description: 学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。
ms.openlocfilehash: b189735340c121a56c48ae21518989cf8e1634f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073618"
---
## <a name="educationidentitymatchingconfiguration-resource-type"></a>educationIdentityMatchingConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学校のデータのプロファイルの id を一致させるための設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリで更新されます。

> **注:** このリソースが選択されている場合は、ユーザーは作成されません。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **matchingOptions** | [educationIdentityMatchingOptions](educationidentitymatchingoptions.md)コレクション | ユーザー アカウントを更新するユーザーを一意に識別に使用するオプションの間のマッピングです。 |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityMatchingConfiguration",
    "matchingOptions": [
        {
            "appliesTo": {"@odata.type": "#microsoft.graph.educationUserRole"},
            "sourcePropertyName": "String",
            "targetPropertyName": "String",
            "targetDomain": "String"
        }
    ]
}
```
