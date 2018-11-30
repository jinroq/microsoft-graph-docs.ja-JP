---
title: educationIdentityCreationConfiguration リソースの種類
description: 学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。
ms.openlocfilehash: edbfa03bb574a1d8d9d4faaa2032ec82f6d20f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073495"
---
## <a name="educationidentitycreationconfiguration-resource-type"></a>educationIdentityCreationConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学校データ プロファイル id の作成時に設定を定義します。 これらの id には、生徒と教師が含まれます。 これらの設定に基づいて、ユーザーがディレクトリに作成されます。

> **注:** ディレクトリ同期がオンになって、設置型の間で同期する Active Directory と Azure Active Directory (AD の Azure) を使っている場合は、 [educationIdentityMatchingConfiguration](educationidentitymatchingconfiguration.md)のリソースを使用してください。

[EducationIdentitySynchronizationConfiguration](educationidentitysynchronizationconfiguration.md)から派生します。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
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