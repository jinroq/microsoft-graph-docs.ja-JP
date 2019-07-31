---
title: office365ActivationsUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 2ced56fdc8f2ed877368163e36588e3d4983d95e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009532"
---
# <a name="office365activationsuserdetail-resource-type"></a>office365ActivationsUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ             | 型                                     | 説明                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | 日付                                     | コンテンツの最新の日付。          |
| userPrincipalName    | String                                   | ユーザーのユーザープリンシパル名 (UPN)。 UPN は、インターネット標準 RFC 822 に基づくユーザーのインターネットスタイルのログイン名です。 規則により、これはユーザーの電子メール名にマップする必要があります。 一般的な形式は、検証済みドメインのテナントのコレクションにドメインが存在する必要がある、エイリアス @ domain です。 このプロパティは、ユーザーの作成時に必要です。 |
| displayName          | 文字列                                   | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 |
| userActivationCounts | [userActivationCounts](../resources/useractivationcounts.md)コレクション | ユーザーの最新の製品ライセンス認証は、割り当てられたすべての製品タイプのすべてのプラットフォームでカウントされます。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
