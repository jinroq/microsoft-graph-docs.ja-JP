---
title: profilePhoto リソースの種類
description: Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。 base 64 でエンコードされていないバイナリ データです。
localization_priority: Priority
ms.openlocfilehash: b1901928a97356b2a9808a446d34981fd74bf456
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579868"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="2d2ee-104">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2d2ee-104">profilePhoto resource type</span></span>
<span data-ttu-id="2d2ee-p102">Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-p102">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="2d2ee-107">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="2d2ee-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d2ee-108">Methods</span></span>

| <span data-ttu-id="2d2ee-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2d2ee-109">Method</span></span>       | <span data-ttu-id="2d2ee-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2d2ee-110">Return Type</span></span>  |<span data-ttu-id="2d2ee-111">説明</span><span class="sxs-lookup"><span data-stu-id="2d2ee-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2d2ee-112">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="2d2ee-112">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="2d2ee-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="2d2ee-113">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="2d2ee-114">指定した **profilePhoto** またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-114">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="2d2ee-115">Update</span><span class="sxs-lookup"><span data-stu-id="2d2ee-115">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="2d2ee-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="2d2ee-116">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="2d2ee-p103">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-p103">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="2d2ee-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2ee-120">Properties</span></span>
| <span data-ttu-id="2d2ee-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d2ee-121">Property</span></span>     | <span data-ttu-id="2d2ee-122">型</span><span class="sxs-lookup"><span data-stu-id="2d2ee-122">Type</span></span>   |<span data-ttu-id="2d2ee-123">説明</span><span class="sxs-lookup"><span data-stu-id="2d2ee-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2d2ee-124">id</span><span class="sxs-lookup"><span data-stu-id="2d2ee-124">id</span></span>|<span data-ttu-id="2d2ee-125">string</span><span class="sxs-lookup"><span data-stu-id="2d2ee-125">string</span></span>|<span data-ttu-id="2d2ee-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-126">Read-only.</span></span>|
|<span data-ttu-id="2d2ee-127">height</span><span class="sxs-lookup"><span data-stu-id="2d2ee-127">height</span></span>|<span data-ttu-id="2d2ee-128">int32</span><span class="sxs-lookup"><span data-stu-id="2d2ee-128">int32</span></span>|<span data-ttu-id="2d2ee-p104">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-p104">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="2d2ee-131">width</span><span class="sxs-lookup"><span data-stu-id="2d2ee-131">width</span></span>|<span data-ttu-id="2d2ee-132">int32</span><span class="sxs-lookup"><span data-stu-id="2d2ee-132">int32</span></span>|<span data-ttu-id="2d2ee-p105">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-p105">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d2ee-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2d2ee-135">Relationships</span></span>
<span data-ttu-id="2d2ee-136">なし</span><span class="sxs-lookup"><span data-stu-id="2d2ee-136">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2d2ee-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2d2ee-137">JSON representation</span></span>

<span data-ttu-id="2d2ee-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2d2ee-138">Here is a JSON representation of the resource.</span></span>

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
