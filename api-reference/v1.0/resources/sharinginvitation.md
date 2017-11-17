---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 75fa8212f77873b86748f6d8f63c8e62c8d6a0ca
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="7aa77-102">SharingInvitation リソース型</span><span class="sxs-lookup"><span data-stu-id="7aa77-102">SharingInvitation resource type</span></span>

<span data-ttu-id="7aa77-103">**SharingInvitation** リソースは、招待に関連するデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="7aa77-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7aa77-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7aa77-104">JSON representation</span></span>

<span data-ttu-id="7aa77-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7aa77-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="7aa77-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7aa77-106">Properties</span></span>

| <span data-ttu-id="7aa77-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="7aa77-107">Property Name</span></span>  | <span data-ttu-id="7aa77-108">型</span><span class="sxs-lookup"><span data-stu-id="7aa77-108">Type</span></span>                          | <span data-ttu-id="7aa77-109">説明</span><span class="sxs-lookup"><span data-stu-id="7aa77-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="7aa77-110">email</span><span class="sxs-lookup"><span data-stu-id="7aa77-110">email</span></span>          | <span data-ttu-id="7aa77-111">String</span><span class="sxs-lookup"><span data-stu-id="7aa77-111">String</span></span>                        | <span data-ttu-id="7aa77-p101">共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7aa77-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="7aa77-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="7aa77-114">invitedBy</span></span>      | [<span data-ttu-id="7aa77-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="7aa77-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="7aa77-p102">このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7aa77-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="7aa77-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="7aa77-118">signInRequired</span></span> | <span data-ttu-id="7aa77-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="7aa77-119">Boolean</span></span>                       | <span data-ttu-id="7aa77-p103">`true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7aa77-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="7aa77-122">備考</span><span class="sxs-lookup"><span data-stu-id="7aa77-122">Remarks</span></span> 

<span data-ttu-id="7aa77-123">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7aa77-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
