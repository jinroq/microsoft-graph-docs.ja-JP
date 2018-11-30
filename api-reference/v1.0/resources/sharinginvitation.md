---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 187a7bd8fe51be57b663c215436272ee711512e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022089"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="280d2-102">SharingInvitation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="280d2-102">SharingInvitation resource type</span></span>

<span data-ttu-id="280d2-103">**SharingInvitation**リソースは、単一の構造に、招待状に関連するデータ項目をグループ化します。</span><span class="sxs-lookup"><span data-stu-id="280d2-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="280d2-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="280d2-104">JSON representation</span></span>

<span data-ttu-id="280d2-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="280d2-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="280d2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="280d2-106">Properties</span></span>

| <span data-ttu-id="280d2-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="280d2-107">Property Name</span></span>  | <span data-ttu-id="280d2-108">型</span><span class="sxs-lookup"><span data-stu-id="280d2-108">Type</span></span>            | <span data-ttu-id="280d2-109">説明</span><span class="sxs-lookup"><span data-stu-id="280d2-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="280d2-110">email</span><span class="sxs-lookup"><span data-stu-id="280d2-110">email</span></span>          | <span data-ttu-id="280d2-111">String</span><span class="sxs-lookup"><span data-stu-id="280d2-111">String</span></span>          | <span data-ttu-id="280d2-p101">共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="280d2-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="280d2-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="280d2-114">invitedBy</span></span>      | <span data-ttu-id="280d2-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="280d2-115">[identitySet][]</span></span> | <span data-ttu-id="280d2-p102">このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="280d2-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="280d2-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="280d2-118">signInRequired</span></span> | <span data-ttu-id="280d2-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="280d2-119">Boolean</span></span>         | <span data-ttu-id="280d2-p103">`true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="280d2-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="280d2-122">備考</span><span class="sxs-lookup"><span data-stu-id="280d2-122">Remarks</span></span>

<span data-ttu-id="280d2-123">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="280d2-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
