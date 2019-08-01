---
title: profilePhoto リソースの種類
description: Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。
localization_priority: Priority
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: baee7eebd3abcaa8376440fb0b20cbe5c69df880
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035057"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="7298f-104">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7298f-104">profilePhoto resource type</span></span>
<span data-ttu-id="7298f-p102">Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="7298f-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="7298f-107">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="7298f-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="7298f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7298f-108">Methods</span></span>

| <span data-ttu-id="7298f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7298f-109">Method</span></span>       | <span data-ttu-id="7298f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7298f-110">Return Type</span></span>  |<span data-ttu-id="7298f-111">説明</span><span class="sxs-lookup"><span data-stu-id="7298f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7298f-112">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="7298f-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="7298f-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7298f-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="7298f-114">指定した **profilePhoto** またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="7298f-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="7298f-115">Update</span><span class="sxs-lookup"><span data-stu-id="7298f-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="7298f-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="7298f-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="7298f-p103">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="7298f-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="7298f-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7298f-120">Properties</span></span>
| <span data-ttu-id="7298f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7298f-121">Property</span></span>     | <span data-ttu-id="7298f-122">型</span><span class="sxs-lookup"><span data-stu-id="7298f-122">Type</span></span>   |<span data-ttu-id="7298f-123">説明</span><span class="sxs-lookup"><span data-stu-id="7298f-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7298f-124">id</span><span class="sxs-lookup"><span data-stu-id="7298f-124">id</span></span>|<span data-ttu-id="7298f-125">string</span><span class="sxs-lookup"><span data-stu-id="7298f-125">string</span></span>|<span data-ttu-id="7298f-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7298f-126">Read-only.</span></span>|
|<span data-ttu-id="7298f-127">height</span><span class="sxs-lookup"><span data-stu-id="7298f-127">height</span></span>|<span data-ttu-id="7298f-128">int32</span><span class="sxs-lookup"><span data-stu-id="7298f-128">int32</span></span>|<span data-ttu-id="7298f-p104">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7298f-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="7298f-131">width</span><span class="sxs-lookup"><span data-stu-id="7298f-131">width</span></span>|<span data-ttu-id="7298f-132">int32</span><span class="sxs-lookup"><span data-stu-id="7298f-132">int32</span></span>|<span data-ttu-id="7298f-p105">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7298f-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7298f-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7298f-135">Relationships</span></span>
<span data-ttu-id="7298f-136">なし</span><span class="sxs-lookup"><span data-stu-id="7298f-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="7298f-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7298f-137">JSON representation</span></span>

<span data-ttu-id="7298f-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7298f-138">Here is a JSON representation of the resource.</span></span>

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
