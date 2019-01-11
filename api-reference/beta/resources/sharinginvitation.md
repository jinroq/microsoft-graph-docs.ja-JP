---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 3ba92573aaef89b1be431ade33caa6ed465917a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835974"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="0c5c3-102">SharingInvitation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c5c3-102">SharingInvitation resource type</span></span>

> <span data-ttu-id="0c5c3-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c5c3-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c5c3-105">**SharingInvitation** リソースは、招待に関連するデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-105">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c5c3-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c5c3-106">JSON representation</span></span>

<span data-ttu-id="0c5c3-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0c5c3-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="0c5c3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c5c3-108">Properties</span></span>

| <span data-ttu-id="0c5c3-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0c5c3-109">Property Name</span></span>  | <span data-ttu-id="0c5c3-110">種類</span><span class="sxs-lookup"><span data-stu-id="0c5c3-110">Type</span></span>                          | <span data-ttu-id="0c5c3-111">説明</span><span class="sxs-lookup"><span data-stu-id="0c5c3-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0c5c3-112">email</span><span class="sxs-lookup"><span data-stu-id="0c5c3-112">email</span></span>          | <span data-ttu-id="0c5c3-113">String</span><span class="sxs-lookup"><span data-stu-id="0c5c3-113">String</span></span>                        | <span data-ttu-id="0c5c3-p102">共有への招待の受信者について指定された電子メール アドレス。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-p102">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="0c5c3-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="0c5c3-116">invitedBy</span></span>      | [<span data-ttu-id="0c5c3-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="0c5c3-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="0c5c3-p103">このアクセス許可を作成した招待状を送信したユーザーに関する情報を提供します (その情報が利用可能な場合)。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-p103">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="0c5c3-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="0c5c3-120">signInRequired</span></span> | <span data-ttu-id="0c5c3-121">ブール値</span><span class="sxs-lookup"><span data-stu-id="0c5c3-121">Boolean</span></span>                       | <span data-ttu-id="0c5c3-p104">`true` の場合、招待状の受信者は共有アイテムにアクセスするためにサインインする必要があります。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-p104">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="0c5c3-124">備考</span><span class="sxs-lookup"><span data-stu-id="0c5c3-124">Remarks</span></span> 

<span data-ttu-id="0c5c3-125">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c5c3-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": ""
}-->
