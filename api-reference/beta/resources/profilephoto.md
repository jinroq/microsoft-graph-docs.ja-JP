---
title: profilePhoto リソースの種類
description: ユーザー、グループまたは Exchange のオンラインまたは Azure Active Directory (AAD) からアクセスする Outlook の連絡先のプロフィールの写真です。 base 64 でエンコードされていないバイナリ データです。
localization_priority: Normal
ms.openlocfilehash: 2a831abd098fb9a0dfa95f6d6dd3a9cd5de128cd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513656"
---
# <a name="profilephoto-resource-type"></a><span data-ttu-id="fed21-104">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fed21-104">profilePhoto resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fed21-105">ユーザー、グループまたは Exchange のオンラインまたは Azure Active Directory (AAD) からアクセスする Outlook の連絡先のプロフィールの写真です。</span><span class="sxs-lookup"><span data-stu-id="fed21-105">A profile photo of a user, group or an Outlook contact accessed from Exchange Online or Azure Active Directory (AAD).</span></span> <span data-ttu-id="fed21-106">base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="fed21-106">It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="fed21-107">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="fed21-107">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> <span data-ttu-id="fed21-108">AAD、上は、任意の次元が写真にできます。</span><span class="sxs-lookup"><span data-stu-id="fed21-108">On AAD, photos can be any dimension.</span></span>

## <a name="methods"></a><span data-ttu-id="fed21-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fed21-109">Methods</span></span>

| <span data-ttu-id="fed21-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="fed21-110">Method</span></span>       | <span data-ttu-id="fed21-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fed21-111">Return Type</span></span>  |<span data-ttu-id="fed21-112">説明</span><span class="sxs-lookup"><span data-stu-id="fed21-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fed21-113">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="fed21-113">Get profilePhoto</span></span>](../api/profilephoto-get.md) | [<span data-ttu-id="fed21-114">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="fed21-114">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="fed21-115">指定した**profilePhoto**またはそのメタデータ (**profilePhoto**プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="fed21-115">Get the specified **profilePhoto** or its metadata (**profilePhoto** properties).</span></span> |
|[<span data-ttu-id="fed21-116">Update</span><span class="sxs-lookup"><span data-stu-id="fed21-116">Update</span></span>](../api/profilephoto-update.md) | [<span data-ttu-id="fed21-117">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="fed21-117">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="fed21-p104">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="fed21-p104">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span> |

## <a name="properties"></a><span data-ttu-id="fed21-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fed21-121">Properties</span></span>
| <span data-ttu-id="fed21-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fed21-122">Property</span></span>     | <span data-ttu-id="fed21-123">型</span><span class="sxs-lookup"><span data-stu-id="fed21-123">Type</span></span>   |<span data-ttu-id="fed21-124">説明</span><span class="sxs-lookup"><span data-stu-id="fed21-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fed21-125">id</span><span class="sxs-lookup"><span data-stu-id="fed21-125">id</span></span>|<span data-ttu-id="fed21-126">string</span><span class="sxs-lookup"><span data-stu-id="fed21-126">string</span></span>|<span data-ttu-id="fed21-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fed21-127">Read-only.</span></span>|
|<span data-ttu-id="fed21-128">height</span><span class="sxs-lookup"><span data-stu-id="fed21-128">height</span></span>|<span data-ttu-id="fed21-129">int32</span><span class="sxs-lookup"><span data-stu-id="fed21-129">int32</span></span>|<span data-ttu-id="fed21-p105">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fed21-p105">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="fed21-132">width</span><span class="sxs-lookup"><span data-stu-id="fed21-132">width</span></span>|<span data-ttu-id="fed21-133">int32</span><span class="sxs-lookup"><span data-stu-id="fed21-133">int32</span></span>|<span data-ttu-id="fed21-p106">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fed21-p106">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fed21-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fed21-136">Relationships</span></span>
<span data-ttu-id="fed21-137">なし</span><span class="sxs-lookup"><span data-stu-id="fed21-137">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fed21-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fed21-138">JSON representation</span></span>

<span data-ttu-id="fed21-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fed21-139">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/profilephoto.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
