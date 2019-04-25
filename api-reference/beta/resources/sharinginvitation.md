---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 0f3acc102762cc1243d8be8362149df1d33717dc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584062"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="03ad1-102">SharingInvitation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="03ad1-102">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03ad1-103">**SharingInvitation** リソースは、招待に関連するデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="03ad1-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03ad1-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="03ad1-104">JSON representation</span></span>

<span data-ttu-id="03ad1-105">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="03ad1-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="03ad1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03ad1-106">Properties</span></span>

| <span data-ttu-id="03ad1-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="03ad1-107">Property Name</span></span>  | <span data-ttu-id="03ad1-108">型</span><span class="sxs-lookup"><span data-stu-id="03ad1-108">Type</span></span>                          | <span data-ttu-id="03ad1-109">説明</span><span class="sxs-lookup"><span data-stu-id="03ad1-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="03ad1-110">email</span><span class="sxs-lookup"><span data-stu-id="03ad1-110">email</span></span>          | <span data-ttu-id="03ad1-111">String</span><span class="sxs-lookup"><span data-stu-id="03ad1-111">String</span></span>                        | <span data-ttu-id="03ad1-p101">共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03ad1-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="03ad1-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="03ad1-114">invitedBy</span></span>      | [<span data-ttu-id="03ad1-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="03ad1-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="03ad1-p102">このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03ad1-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="03ad1-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="03ad1-118">signInRequired</span></span> | <span data-ttu-id="03ad1-119">ブール値</span><span class="sxs-lookup"><span data-stu-id="03ad1-119">Boolean</span></span>                       | <span data-ttu-id="03ad1-p103">`true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="03ad1-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="03ad1-122">備考</span><span class="sxs-lookup"><span data-stu-id="03ad1-122">Remarks</span></span> 

<span data-ttu-id="03ad1-123">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03ad1-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinginvitation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
