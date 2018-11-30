---
title: profilePhoto リソースの種類
description: Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。
ms.openlocfilehash: c5f74e1dcd48e42a2e17d5a64e6ed4b9e9cca5e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024191"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="96600-104">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96600-104">profilePhoto resource type</span></span>
<span data-ttu-id="96600-p102">Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="96600-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="96600-107">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="96600-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="96600-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="96600-108">Methods</span></span>

| <span data-ttu-id="96600-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="96600-109">Method</span></span>       | <span data-ttu-id="96600-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="96600-110">Return Type</span></span>  |<span data-ttu-id="96600-111">説明</span><span class="sxs-lookup"><span data-stu-id="96600-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96600-112">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="96600-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="96600-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="96600-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="96600-114">指定した **profilePhoto** またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="96600-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="96600-115">Update</span><span class="sxs-lookup"><span data-stu-id="96600-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="96600-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="96600-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="96600-p103">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="96600-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="96600-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96600-120">Properties</span></span>
| <span data-ttu-id="96600-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96600-121">Property</span></span>     | <span data-ttu-id="96600-122">型</span><span class="sxs-lookup"><span data-stu-id="96600-122">Type</span></span>   |<span data-ttu-id="96600-123">説明</span><span class="sxs-lookup"><span data-stu-id="96600-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96600-124">ID</span><span class="sxs-lookup"><span data-stu-id="96600-124">id</span></span>|<span data-ttu-id="96600-125">文字列</span><span class="sxs-lookup"><span data-stu-id="96600-125">string</span></span>|<span data-ttu-id="96600-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96600-126">Read-only.</span></span>|
|<span data-ttu-id="96600-127">height</span><span class="sxs-lookup"><span data-stu-id="96600-127">height</span></span>|<span data-ttu-id="96600-128">int32</span><span class="sxs-lookup"><span data-stu-id="96600-128">int32</span></span>|<span data-ttu-id="96600-p104">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96600-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="96600-131">width</span><span class="sxs-lookup"><span data-stu-id="96600-131">width</span></span>|<span data-ttu-id="96600-132">int32</span><span class="sxs-lookup"><span data-stu-id="96600-132">int32</span></span>|<span data-ttu-id="96600-p105">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96600-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96600-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="96600-135">Relationships</span></span>
<span data-ttu-id="96600-136">なし</span><span class="sxs-lookup"><span data-stu-id="96600-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="96600-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96600-137">JSON representation</span></span>

<span data-ttu-id="96600-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96600-138">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
