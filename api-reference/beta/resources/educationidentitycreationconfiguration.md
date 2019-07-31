---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データプロファイル id の作成に関する設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内に作成されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 09d36a87b8ed1485ce112d40ca8b920290e23997
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006382"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

学校データプロファイル id の作成に関する設定を定義します。 これらの id には、学生と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリ内に作成されます。

> **注:** オンプレミスの Active Directory と Azure Active Directory (Azure AD) との間でディレクトリ同期をオンにしている場合は、代わりに[educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)リソースを使用します。

[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md)コレクション |  ユーザーの種類ごとに使用するドメインのリストを設定します。  |


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
