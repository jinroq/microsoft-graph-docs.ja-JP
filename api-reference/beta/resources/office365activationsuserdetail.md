---
title: office365ActivationsUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 3e2b7d5fb3c42db02407a187649544b2560f898a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982856"
---
# <a name="office365activationsuserdetail-resource-type"></a>office365ActivationsUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ             | 種類                                     | 説明                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | 日付                                     | コンテンツの最新の日付。          |
| userPrincipalName    | String                                   | ユーザー プリンシパル名 (UPN) のユーザーです。 UPN は、インターネット標準の RFC 822 に基づくユーザーに対して、インターネット スタイルのログイン名です。 規則では、これはユーザーの電子メール名にマップする必要があります。 一般的な形式は、ドメインをドメインの検証済みのテナントのコレクション内に存在する必要があります、alias@domain、です。 このプロパティは、ユーザーの作成時に必要です。 |
| displayName          | String                                   | アドレス帳に表示されるユーザーの名前。 これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせになります。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 |
| userActivationCounts | [userActivationCounts](../resources/useractivationcounts.md)コレクション | ユーザーの最新の製品ライセンス認証は、すべての割り当てられている製品の種類のすべてのプラットフォーム上でカウントします。 |

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
