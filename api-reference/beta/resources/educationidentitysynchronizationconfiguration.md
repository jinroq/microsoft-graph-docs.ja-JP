---
title: educationIdentitySynchronizationConfiguration リソースの種類
description: すべての学校データプロファイル id 同期構成の抽象基本クラス。 派生クラスは、id を同期するための動作を定義します。 派生型を次に示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 713bb285e739d9182a982f02975a9b9f46761e3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736517"
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

