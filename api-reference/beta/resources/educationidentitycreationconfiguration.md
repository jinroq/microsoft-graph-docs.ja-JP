---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データプロファイル id の作成に関する設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内に作成されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: e35eed699e1a1439fd94c251e560be902f96bd09
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340562"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校データプロファイル id の作成に関する設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内に作成されます。

> **注:** オンプレミスの Active directory と azure active directory (azure AD) との間でディレクトリ同期をオンにしている場合は、代わりに[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)リソースを使用します。

[educationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **userdomains** | [educationIdentityDomain](educationidentitydomain.md)コレクション |  ユーザーの種類ごとに使用するドメインのリストを設定します。  |


## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
