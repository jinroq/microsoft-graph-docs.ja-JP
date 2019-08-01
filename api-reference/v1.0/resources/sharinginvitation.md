---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: SharingInvitation リソースは、招待に関連するデータ項目を1つの構造体にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 011402b40b601642a048b91e3b3f66de0792aaf2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034245"
---
# <a name="sharinginvitation-resource-type"></a>SharingInvitation リソースの種類

**Sharinginvitation**リソースは、招待に関連するデータ項目を1つの構造体にグループ化します。

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
| メール          | String          | 共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。
| invitedBy      | [identitySet][] | このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。
| signInRequired | ブール値         | `true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。

## <a name="remarks"></a>備考

DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
