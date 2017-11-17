---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SpecialFolder
ms.openlocfilehash: 84e67df8aae6e72363d4ba148e92f9046f41bb29
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="bc0e4-102">SpecialFolder リソース型</span><span class="sxs-lookup"><span data-stu-id="bc0e4-102">SpecialFolder resource type</span></span>

<span data-ttu-id="bc0e4-103">**SpecialFolder** リソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="bc0e4-104">**DriveItem** が null 以外の **specialFolder** ファセットを持つ場合、その項目は特殊な (名前が付けられた) フォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a specail (named) folder. Special folders can be accessed directly via the special folders collection.</span></span>
<span data-ttu-id="bc0e4-105">特殊なフォルダーは [特殊なフォルダーのコレクション](../api/drive_get_specialfolder.md) 経由で直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-105">If a DriveItem has a non-null specialFolder facet, the item represents a specail (named) folder. Special folders can be accessed directly via the [special folders collection](../api/drive_get_specialfolder.md).</span></span>

<span data-ttu-id="bc0e4-p102">特殊なフォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊なフォルダーが名前変更されたりドライブ内の別の場所に移動されたりした場合、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="bc0e4-p103">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="bc0e4-110">**注:** アプリが **Files.Read** スコープのみを要求していて、存在しない特殊なフォルダーを要求する場合、返答は `403 Forbidden` エラーになります。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc0e4-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc0e4-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bc0e4-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc0e4-112">Properties</span></span>

| <span data-ttu-id="bc0e4-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc0e4-113">Property</span></span>  | <span data-ttu-id="bc0e4-114">型</span><span class="sxs-lookup"><span data-stu-id="bc0e4-114">Type</span></span>   | <span data-ttu-id="bc0e4-115">説明</span><span class="sxs-lookup"><span data-stu-id="bc0e4-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="bc0e4-116">name</span><span class="sxs-lookup"><span data-stu-id="bc0e4-116">name</span></span>      | <span data-ttu-id="bc0e4-117">string</span><span class="sxs-lookup"><span data-stu-id="bc0e4-117">string</span></span> | <span data-ttu-id="bc0e4-118">`/drive/special` コレクション内のこの項目の一意識別子</span><span class="sxs-lookup"><span data-stu-id="bc0e4-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="bc0e4-119">特殊なフォルダー</span><span class="sxs-lookup"><span data-stu-id="bc0e4-119">Special folders</span></span>

<span data-ttu-id="bc0e4-120">以下は OneDrive Personal および OneDrive for Business で利用可能な特殊なフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="bc0e4-121">名前</span><span class="sxs-lookup"><span data-stu-id="bc0e4-121">Name</span></span>        | <span data-ttu-id="bc0e4-122">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="bc0e4-122">Folder id</span></span>    | <span data-ttu-id="bc0e4-123">説明</span><span class="sxs-lookup"><span data-stu-id="bc0e4-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="bc0e4-124">App Root</span><span class="sxs-lookup"><span data-stu-id="bc0e4-124">App Root</span></span>    | `approot`    | <span data-ttu-id="bc0e4-p104">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="bc0e4-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="bc0e4-127">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="bc0e4-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="bc0e4-p105">カメラ ロールのバックアップ フォルダー。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="bc0e4-130">ドキュメント</span><span class="sxs-lookup"><span data-stu-id="bc0e4-130">Documents</span></span>   | `documents`  | <span data-ttu-id="bc0e4-131">ドキュメント フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="bc0e4-132">Music</span><span class="sxs-lookup"><span data-stu-id="bc0e4-132">Music</span></span>       | `music`      | <span data-ttu-id="bc0e4-p106">ミュージック フォルダーです。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="bc0e4-135">Photos</span><span class="sxs-lookup"><span data-stu-id="bc0e4-135">Photos</span></span>      | `photos`     | <span data-ttu-id="bc0e4-136">フォト フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="bc0e4-137">備考</span><span class="sxs-lookup"><span data-stu-id="bc0e4-137">Remarks</span></span> 

<span data-ttu-id="bc0e4-138">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc0e4-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
