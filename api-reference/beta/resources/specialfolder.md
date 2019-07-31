---
author: JeremyKelley
description: SpecialFolderリソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 647916e53409be47ebd3547a8712778bb6ba9f54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008076"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="e298d-103">SpecialFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e298d-103">SpecialFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e298d-104">**SpecialFolder**リソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="e298d-104">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="e298d-105">**DriveItem** が null 以外の **specialFolder** ファセットを持つ場合、その項目は特殊な (名前が付けられた) フォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="e298d-105">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="e298d-106">特殊なフォルダーは [特殊なフォルダーのコレクション](../api/drive-get-specialfolder.md) 経由で直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e298d-106">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="e298d-p102">特殊なフォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊なフォルダーが名前変更されたりドライブ内の別の場所に移動されたりした場合、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="e298d-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="e298d-p103">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="e298d-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="e298d-111">**注:** アプリが **Files.Read** スコープのみを要求していて、存在しない特殊なフォルダーを要求する場合、返答は `403 Forbidden` エラーになります。</span><span class="sxs-lookup"><span data-stu-id="e298d-111">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e298d-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e298d-112">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.specialFolder"
}-->
```json
{
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="e298d-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e298d-113">Properties</span></span>

| <span data-ttu-id="e298d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e298d-114">Property</span></span>  | <span data-ttu-id="e298d-115">型</span><span class="sxs-lookup"><span data-stu-id="e298d-115">Type</span></span>   | <span data-ttu-id="e298d-116">説明</span><span class="sxs-lookup"><span data-stu-id="e298d-116">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="e298d-117">name</span><span class="sxs-lookup"><span data-stu-id="e298d-117">name</span></span>      | <span data-ttu-id="e298d-118">string</span><span class="sxs-lookup"><span data-stu-id="e298d-118">string</span></span> | <span data-ttu-id="e298d-119">`/drive/special` コレクション内のこの項目の一意識別子</span><span class="sxs-lookup"><span data-stu-id="e298d-119">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="e298d-120">特殊なフォルダー</span><span class="sxs-lookup"><span data-stu-id="e298d-120">Special folders</span></span>

<span data-ttu-id="e298d-121">以下は OneDrive Personal および OneDrive for Business で利用可能な特殊なフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="e298d-121">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="e298d-122">名前</span><span class="sxs-lookup"><span data-stu-id="e298d-122">Name</span></span>        | <span data-ttu-id="e298d-123">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="e298d-123">Folder id</span></span>    | <span data-ttu-id="e298d-124">説明</span><span class="sxs-lookup"><span data-stu-id="e298d-124">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="e298d-125">App Root</span><span class="sxs-lookup"><span data-stu-id="e298d-125">App Root</span></span>    | `approot`    | <span data-ttu-id="e298d-p104">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="e298d-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="e298d-128">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="e298d-128">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="e298d-p105">カメラ ロールのバックアップ フォルダー。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="e298d-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="e298d-131">Documents</span><span class="sxs-lookup"><span data-stu-id="e298d-131">Documents</span></span>   | `documents`  | <span data-ttu-id="e298d-132">ドキュメント フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="e298d-132">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="e298d-133">Music</span><span class="sxs-lookup"><span data-stu-id="e298d-133">Music</span></span>       | `music`      | <span data-ttu-id="e298d-p106">ミュージック フォルダーです。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="e298d-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="e298d-136">Photos</span><span class="sxs-lookup"><span data-stu-id="e298d-136">Photos</span></span>      | `photos`     | <span data-ttu-id="e298d-137">フォト フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="e298d-137">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="e298d-138">備考</span><span class="sxs-lookup"><span data-stu-id="e298d-138">Remarks</span></span> 

<span data-ttu-id="e298d-139">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e298d-139">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
