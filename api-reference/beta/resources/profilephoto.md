---
title: profilePhoto リソースの種類
description: ユーザー、グループまたは Exchange のオンラインまたは Azure Active Directory (AAD) からアクセスする Outlook の連絡先のプロフィールの写真です。 base 64 でエンコードされていないバイナリ データです。
ms.openlocfilehash: 61123542ce66c1e999fb6d90c154a78dbb77df50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067573"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="9ac27-104">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ac27-104">profilePhoto resource type</span></span>

> <span data-ttu-id="9ac27-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ac27-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9ac27-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ac27-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9ac27-107">ユーザー、グループまたは Exchange のオンラインまたは Azure Active Directory (AAD) からアクセスする Outlook の連絡先のプロフィールの写真です。</span><span class="sxs-lookup"><span data-stu-id="9ac27-107">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="9ac27-108">base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="9ac27-108">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="9ac27-109">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="9ac27-109">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="9ac27-110">AAD、上は、任意の次元が写真にできます。</span><span class="sxs-lookup"><span data-stu-id="9ac27-110">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="9ac27-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ac27-111">Methods</span></span>

| <span data-ttu-id="9ac27-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="9ac27-112">Method</span></span>       | <span data-ttu-id="9ac27-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9ac27-113">Return Type</span></span>  |<span data-ttu-id="9ac27-114">説明</span><span class="sxs-lookup"><span data-stu-id="9ac27-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ac27-115">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="9ac27-115">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="9ac27-116">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9ac27-116">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="9ac27-117">指定した**profilePhoto**またはそのメタデータ (**profilePhoto**プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="9ac27-117">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="9ac27-118">Update</span><span class="sxs-lookup"><span data-stu-id="9ac27-118">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="9ac27-119">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="9ac27-119">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="9ac27-p105">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="9ac27-p105">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="9ac27-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ac27-123">Properties</span></span>
| <span data-ttu-id="9ac27-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ac27-124">Property</span></span>     | <span data-ttu-id="9ac27-125">型</span><span class="sxs-lookup"><span data-stu-id="9ac27-125">Type</span></span>   |<span data-ttu-id="9ac27-126">説明</span><span class="sxs-lookup"><span data-stu-id="9ac27-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ac27-127">ID</span><span class="sxs-lookup"><span data-stu-id="9ac27-127">id</span></span>|<span data-ttu-id="9ac27-128">文字列</span><span class="sxs-lookup"><span data-stu-id="9ac27-128">string</span></span>|<span data-ttu-id="9ac27-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ac27-129">Read-only.</span></span>|
|<span data-ttu-id="9ac27-130">height</span><span class="sxs-lookup"><span data-stu-id="9ac27-130">height</span></span>|<span data-ttu-id="9ac27-131">int32</span><span class="sxs-lookup"><span data-stu-id="9ac27-131">int32</span></span>|<span data-ttu-id="9ac27-p106">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ac27-p106">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="9ac27-134">width</span><span class="sxs-lookup"><span data-stu-id="9ac27-134">width</span></span>|<span data-ttu-id="9ac27-135">int32</span><span class="sxs-lookup"><span data-stu-id="9ac27-135">int32</span></span>|<span data-ttu-id="9ac27-p107">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9ac27-p107">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ac27-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9ac27-138">Relationships</span></span>
<span data-ttu-id="9ac27-139">なし</span><span class="sxs-lookup"><span data-stu-id="9ac27-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9ac27-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ac27-140">JSON representation</span></span>

<span data-ttu-id="9ac27-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9ac27-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
