---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべての学校データプロファイル id 同期構成の抽象基本クラス。 派生クラスは、id を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e282a9701eaae04aae33d9fd9efc9b86f7df3635
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972678"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a>educationIdentitySynchronizationConfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

すべての学校データプロファイル id 同期構成の抽象基本クラス。 派生クラスは、id を同期するための動作を定義します。 派生型を次に示します。

## <a name="derived-types"></a>派生型
| 型 | 説明 |
|:-|:-|
| [**educationIdentityMatchingConfiguration**](educationidentitymatchingconfiguration.md) | この種類を使用して、Azure Active Directory (Azure AD) の既存のユーザーアカウントと照合します。 |
| [**educationIdentityCreationConfiguration**](educationidentitycreationconfiguration.md) | この種類を使用して、Azure AD で新しいユーザーアカウントを作成します。 |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
   "isAbstract":true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
}-->

```json
{
}
```

