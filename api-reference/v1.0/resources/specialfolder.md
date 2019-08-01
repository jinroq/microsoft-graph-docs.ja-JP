---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
description: SpecialFolderリソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e7b5878d091e766ffa5a591c3ea72e4abcad9461
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034035"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="38a94-103">SpecialFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="38a94-103">SpecialFolder resource type</span></span>

<span data-ttu-id="38a94-104">**SpecialFolder**リソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="38a94-104">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="38a94-105">**DriveItem** が null 以外の **specialFolder** ファセットを持つ場合、その項目は特殊な (名前が付けられた) フォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="38a94-105">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="38a94-106">特殊なフォルダーは [特殊なフォルダーのコレクション](../api/drive-get-specialfolder.md) 経由で直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="38a94-106">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="38a94-p102">特殊なフォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊なフォルダーが名前変更されたりドライブ内の別の場所に移動されたりした場合、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="38a94-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="38a94-p103">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="38a94-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="38a94-111">**注:** アプリが **Files.Read** スコープのみを要求していて、存在しない特殊なフォルダーを要求する場合、返答は `403 Forbidden` エラーになります。</span><span class="sxs-lookup"><span data-stu-id="38a94-111">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38a94-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="38a94-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="38a94-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38a94-113">Properties</span></span>

| <span data-ttu-id="38a94-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38a94-114">Property</span></span>  | <span data-ttu-id="38a94-115">型</span><span class="sxs-lookup"><span data-stu-id="38a94-115">Type</span></span>   | <span data-ttu-id="38a94-116">説明</span><span class="sxs-lookup"><span data-stu-id="38a94-116">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="38a94-117">name</span><span class="sxs-lookup"><span data-stu-id="38a94-117">name</span></span>      | <span data-ttu-id="38a94-118">string</span><span class="sxs-lookup"><span data-stu-id="38a94-118">string</span></span> | <span data-ttu-id="38a94-119">`/drive/special` コレクション内のこの項目の一意識別子</span><span class="sxs-lookup"><span data-stu-id="38a94-119">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="38a94-120">特殊なフォルダー</span><span class="sxs-lookup"><span data-stu-id="38a94-120">Special folders</span></span>

<span data-ttu-id="38a94-121">以下は OneDrive Personal および OneDrive for Business で利用可能な特殊なフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="38a94-121">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="38a94-122">名前</span><span class="sxs-lookup"><span data-stu-id="38a94-122">Name</span></span>        | <span data-ttu-id="38a94-123">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="38a94-123">Folder id</span></span>    | <span data-ttu-id="38a94-124">説明</span><span class="sxs-lookup"><span data-stu-id="38a94-124">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="38a94-125">App Root</span><span class="sxs-lookup"><span data-stu-id="38a94-125">App Root</span></span>    | `approot`    | <span data-ttu-id="38a94-p104">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="38a94-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="38a94-128">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="38a94-128">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="38a94-p105">カメラ ロールのバックアップ フォルダー。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="38a94-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="38a94-131">Documents</span><span class="sxs-lookup"><span data-stu-id="38a94-131">Documents</span></span>   | `documents`  | <span data-ttu-id="38a94-132">ドキュメント フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="38a94-132">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="38a94-133">Music</span><span class="sxs-lookup"><span data-stu-id="38a94-133">Music</span></span>       | `music`      | <span data-ttu-id="38a94-p106">ミュージック フォルダーです。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="38a94-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="38a94-136">Photos</span><span class="sxs-lookup"><span data-stu-id="38a94-136">Photos</span></span>      | `photos`     | <span data-ttu-id="38a94-137">フォト フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="38a94-137">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="38a94-138">備考</span><span class="sxs-lookup"><span data-stu-id="38a94-138">Remarks</span></span> 

<span data-ttu-id="38a94-139">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38a94-139">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The SpecialFolder facet provides information about folders accessible as special folders.",
  "keywords": "special folder,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SpecialFolder"
} -->
