---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 9237c401fd83a7b30303f147402262c022b820a7
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23265856"
---
# <a name="sharinginvitation-resource-type"></a>SharingInvitation リソース型

**SharingInvitation** リソースは、招待に関連するデータ項目を 1 つの構造にグループ化します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}
```

## <a name="properties"></a>プロパティ

| プロパティ名  | 型            | 説明
|:---------------|:----------------|:------------------------------------------
| 電子メールを送信する          | 文字列          | 共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。
| invitedBy      | [identitySet][] | このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。
| signInRequired | ブール値         | の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。`true`

## <a name="remarks"></a>備考

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

[DriveItem]: driveItem.md
[IdentitySet]: identitySet.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
