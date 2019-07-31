---
title: profilePhoto リソースの種類
description: Exchange Online または Azure Active Directory (AAD) からアクセスされるユーザー、グループ、または Outlook 連絡先のプロファイル写真。 base 64 でエンコードされていないバイナリ データです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: eee47378343aef1b0a471ac186099d4598124862
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965678"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="43bdb-104">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43bdb-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43bdb-105">Exchange Online または Azure Active Directory (AAD) からアクセスされるユーザー、グループ、または Outlook 連絡先のプロファイル写真。</span><span class="sxs-lookup"><span data-stu-id="43bdb-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="43bdb-106">base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="43bdb-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="43bdb-107">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="43bdb-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="43bdb-108">AAD では、写真は任意の次元にすることができます。</span><span class="sxs-lookup"><span data-stu-id="43bdb-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="43bdb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="43bdb-109">Methods</span></span>

| <span data-ttu-id="43bdb-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="43bdb-110">Method</span></span>       | <span data-ttu-id="43bdb-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="43bdb-111">Return Type</span></span>  |<span data-ttu-id="43bdb-112">説明</span><span class="sxs-lookup"><span data-stu-id="43bdb-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43bdb-113">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="43bdb-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="43bdb-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="43bdb-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="43bdb-115">指定した **profilePhoto** またはそのメタデータ (**profilePhoto** プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="43bdb-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="43bdb-116">Update</span><span class="sxs-lookup"><span data-stu-id="43bdb-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="43bdb-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="43bdb-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="43bdb-p104">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="43bdb-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="43bdb-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43bdb-121">Properties</span></span>
| <span data-ttu-id="43bdb-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43bdb-122">Property</span></span>     | <span data-ttu-id="43bdb-123">型</span><span class="sxs-lookup"><span data-stu-id="43bdb-123">Type</span></span>   |<span data-ttu-id="43bdb-124">説明</span><span class="sxs-lookup"><span data-stu-id="43bdb-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43bdb-125">id</span><span class="sxs-lookup"><span data-stu-id="43bdb-125">id</span></span>|<span data-ttu-id="43bdb-126">string</span><span class="sxs-lookup"><span data-stu-id="43bdb-126">string</span></span>|<span data-ttu-id="43bdb-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="43bdb-127">Read-only.</span></span>|
|<span data-ttu-id="43bdb-128">height</span><span class="sxs-lookup"><span data-stu-id="43bdb-128">height</span></span>|<span data-ttu-id="43bdb-129">int32</span><span class="sxs-lookup"><span data-stu-id="43bdb-129">int32</span></span>|<span data-ttu-id="43bdb-p105">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="43bdb-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="43bdb-132">width</span><span class="sxs-lookup"><span data-stu-id="43bdb-132">width</span></span>|<span data-ttu-id="43bdb-133">int32</span><span class="sxs-lookup"><span data-stu-id="43bdb-133">int32</span></span>|<span data-ttu-id="43bdb-p106">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="43bdb-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43bdb-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43bdb-136">Relationships</span></span>
<span data-ttu-id="43bdb-137">なし</span><span class="sxs-lookup"><span data-stu-id="43bdb-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="43bdb-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43bdb-138">JSON representation</span></span>

<span data-ttu-id="43bdb-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43bdb-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
