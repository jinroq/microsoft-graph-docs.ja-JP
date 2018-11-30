---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: ba909158ce0ba28b6af20b8dbff858c65f07cbe9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072524"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="fe763-102">SharingInvitation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe763-102">SharingInvitation resource type</span></span>

> <span data-ttu-id="fe763-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe763-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe763-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe763-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe763-105">**SharingInvitation** リソースは、招待に関連するデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="fe763-105">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe763-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe763-106">JSON representation</span></span>

<span data-ttu-id="fe763-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fe763-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="fe763-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe763-108">Properties</span></span>

| <span data-ttu-id="fe763-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="fe763-109">Property Name</span></span>  | <span data-ttu-id="fe763-110">型</span><span class="sxs-lookup"><span data-stu-id="fe763-110">Type</span></span>                          | <span data-ttu-id="fe763-111">説明</span><span class="sxs-lookup"><span data-stu-id="fe763-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fe763-112">email</span><span class="sxs-lookup"><span data-stu-id="fe763-112">email</span></span>          | <span data-ttu-id="fe763-113">String</span><span class="sxs-lookup"><span data-stu-id="fe763-113">String</span></span>                        | <span data-ttu-id="fe763-p102">共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fe763-p102">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="fe763-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="fe763-116">invitedBy</span></span>      | [<span data-ttu-id="fe763-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe763-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="fe763-p103">このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fe763-p103">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="fe763-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="fe763-120">signInRequired</span></span> | <span data-ttu-id="fe763-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="fe763-121">Boolean</span></span>                       | <span data-ttu-id="fe763-p104">`true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fe763-p104">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="fe763-124">備考</span><span class="sxs-lookup"><span data-stu-id="fe763-124">Remarks</span></span> 

<span data-ttu-id="fe763-125">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe763-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
