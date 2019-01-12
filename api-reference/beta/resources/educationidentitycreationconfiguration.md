---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: cb7d3d101c547f1ced1b16bf857b7a7e953dc91b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912751"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。

> **注:** ディレクトリ同期がオンになって、設置型の間で同期する Active Directory と Azure Active Directory (AD の Azure) を使っている場合は、 [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)のリソースを使用してください。

[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **userDomains** | [educationIdentityDomain](educationidentitydomain.md)コレクション |  ユーザーの種類ごとに使用するドメインの一覧を設定します。  |


## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
    "userDomains": [
        {
            "@odata.type": "#microsoft.graph.educationIdentityDomain",
        }
    ]
}
```
