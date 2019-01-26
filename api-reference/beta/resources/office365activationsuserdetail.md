---
title: office365ActivationsUserDetail リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: a3561768e36fc63c779e19a9aa05863dd9af9315
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576886"
---
# <a name="office365activationsuserdetail-resource-type"></a>office365ActivationsUserDetail リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ             | 型                                     | 説明                              |
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
