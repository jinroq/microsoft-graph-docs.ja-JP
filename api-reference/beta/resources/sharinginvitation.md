---
author: JeremyKelley
description: SharingInvitation リソースは、招待に関連するデータ項目を1つの構造体にグループ化します。
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: eebfa17a08918ec3ac08700577921b1037761086
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008335"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="4d843-103">SharingInvitation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4d843-103">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d843-104">**Sharinginvitation**リソースは、招待に関連するデータ項目を1つの構造体にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="4d843-104">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4d843-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4d843-105">JSON representation</span></span>

<span data-ttu-id="4d843-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4d843-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="4d843-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4d843-107">Properties</span></span>

| <span data-ttu-id="4d843-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4d843-108">Property Name</span></span>  | <span data-ttu-id="4d843-109">型</span><span class="sxs-lookup"><span data-stu-id="4d843-109">Type</span></span>                          | <span data-ttu-id="4d843-110">説明</span><span class="sxs-lookup"><span data-stu-id="4d843-110">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4d843-111">メール</span><span class="sxs-lookup"><span data-stu-id="4d843-111">email</span></span>          | <span data-ttu-id="4d843-112">String</span><span class="sxs-lookup"><span data-stu-id="4d843-112">String</span></span>                        | <span data-ttu-id="4d843-p101">共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d843-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="4d843-115">invitedBy</span><span class="sxs-lookup"><span data-stu-id="4d843-115">invitedBy</span></span>      | [<span data-ttu-id="4d843-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="4d843-116">identitySet</span></span>](identityset.md) | <span data-ttu-id="4d843-p102">このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d843-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="4d843-119">signInRequired</span><span class="sxs-lookup"><span data-stu-id="4d843-119">signInRequired</span></span> | <span data-ttu-id="4d843-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="4d843-120">Boolean</span></span>                       | <span data-ttu-id="4d843-p103">`true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4d843-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="4d843-123">備考</span><span class="sxs-lookup"><span data-stu-id="4d843-123">Remarks</span></span> 

<span data-ttu-id="4d843-124">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d843-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
