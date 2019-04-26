---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SpecialFolder
localization_priority: Normal
ms.openlocfilehash: d30c1169d859bdb9299744b92efc6ab737c20851
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563729"
---
# <a name="specialfolder-resource-type"></a><span data-ttu-id="24ec8-102">SpecialFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24ec8-102">SpecialFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24ec8-103">**SpecialFolder**リソースは、特殊フォルダー関連のデータ項目を単一の構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="24ec8-103">The **SpecialFolder** resource groups special folder-related data items into a single structure.</span></span>

<span data-ttu-id="24ec8-104">**DriveItem** が null 以外の **specialFolder** ファセットを持つ場合、その項目は特殊な (名前が付けられた) フォルダーを示します。</span><span class="sxs-lookup"><span data-stu-id="24ec8-104">If a **DriveItem** has a non-null **specialFolder** facet, the item represents a special (named) folder.</span></span>
<span data-ttu-id="24ec8-105">特殊なフォルダーは [特殊なフォルダーのコレクション](../api/drive-get-specialfolder.md) 経由で直接アクセスできます。</span><span class="sxs-lookup"><span data-stu-id="24ec8-105">Special folders can be accessed directly via the [special folders collection](../api/drive-get-specialfolder.md).</span></span>

<span data-ttu-id="24ec8-p102">特殊なフォルダーは、フォルダーを (ローカライズが必要となる) パスで探したり、ID を持つフォルダーを参照したりせずに、既知のフォルダーにアクセスするための、単純なエイリアスを提供します。特殊なフォルダーが名前変更されたりドライブ内の別の場所に移動されたりした場合、この構文はそのフォルダーを返し続けます。</span><span class="sxs-lookup"><span data-stu-id="24ec8-p102">Special folders provide simple aliases to access well-known folders without the need to look up the folder by path (which would require localization), or reference the folder with an ID. If a special folder is renamed or moved to another location within the drive, this syntax will continue to return that folder.</span></span>

<span data-ttu-id="24ec8-p103">特殊なフォルダーは、まだ存在していない場合、アプリケーションが最初に書き込みを試行したときに自動的に作成されます。ユーザーが削除した場合は、もう一度書き込まれたときに再作成されます。</span><span class="sxs-lookup"><span data-stu-id="24ec8-p103">Special folders are automatically created the first time an application attempts to write to one, if it doesn't already exist. If a user deletes one, it is recreated when written to again.</span></span>

<span data-ttu-id="24ec8-110">**注:** アプリが **Files.Read** スコープのみを要求していて、存在しない特殊なフォルダーを要求する場合、返答は `403 Forbidden` エラーになります。</span><span class="sxs-lookup"><span data-stu-id="24ec8-110">**Note:** If your app has only requested **Files.Read** scope and requests a special folder that doesn't exist, the response will be a `403 Forbidden` error.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24ec8-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24ec8-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="24ec8-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24ec8-112">Properties</span></span>

| <span data-ttu-id="24ec8-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24ec8-113">Property</span></span>  | <span data-ttu-id="24ec8-114">型</span><span class="sxs-lookup"><span data-stu-id="24ec8-114">Type</span></span>   | <span data-ttu-id="24ec8-115">説明</span><span class="sxs-lookup"><span data-stu-id="24ec8-115">Description</span></span>                                                            |
|:----------|:-------|:-----------------------------------------------------------------------|
| <span data-ttu-id="24ec8-116">name</span><span class="sxs-lookup"><span data-stu-id="24ec8-116">name</span></span>      | <span data-ttu-id="24ec8-117">string</span><span class="sxs-lookup"><span data-stu-id="24ec8-117">string</span></span> | <span data-ttu-id="24ec8-118">`/drive/special` コレクション内のこの項目の一意識別子</span><span class="sxs-lookup"><span data-stu-id="24ec8-118">The unique identifier for this item in the `/drive/special` collection</span></span> |

## <a name="special-folders"></a><span data-ttu-id="24ec8-119">特殊なフォルダー</span><span class="sxs-lookup"><span data-stu-id="24ec8-119">Special folders</span></span>

<span data-ttu-id="24ec8-120">以下は OneDrive Personal および OneDrive for Business で利用可能な特殊なフォルダーです。</span><span class="sxs-lookup"><span data-stu-id="24ec8-120">Here are the special folders available in OneDrive Personal and OneDrive for Business.</span></span>

| <span data-ttu-id="24ec8-121">名前</span><span class="sxs-lookup"><span data-stu-id="24ec8-121">Name</span></span>        | <span data-ttu-id="24ec8-122">フォルダー ID</span><span class="sxs-lookup"><span data-stu-id="24ec8-122">Folder id</span></span>    | <span data-ttu-id="24ec8-123">説明</span><span class="sxs-lookup"><span data-stu-id="24ec8-123">Description</span></span>                                                              |
|:------------|:-------------|:-------------------------------------------------------------------------|
| <span data-ttu-id="24ec8-124">App Root</span><span class="sxs-lookup"><span data-stu-id="24ec8-124">App Root</span></span>    | `approot`    | <span data-ttu-id="24ec8-p104">そのアプリケーションの個人用フォルダー。通常は `/Apps/{Application Name}` 内</span><span class="sxs-lookup"><span data-stu-id="24ec8-p104">The application's personal folder. Usually in `/Apps/{Application Name}`</span></span> |
| <span data-ttu-id="24ec8-127">Camera Roll</span><span class="sxs-lookup"><span data-stu-id="24ec8-127">Camera Roll</span></span> | `cameraroll` | <span data-ttu-id="24ec8-p105">カメラ ロールのバックアップ フォルダー。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="24ec8-p105">The Camera Roll Backup folder. Not available in OneDrive for Business.</span></span>   |
| <span data-ttu-id="24ec8-130">Documents</span><span class="sxs-lookup"><span data-stu-id="24ec8-130">Documents</span></span>   | `documents`  | <span data-ttu-id="24ec8-131">ドキュメント フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="24ec8-131">The Documents folder.</span></span>                                                    |
| <span data-ttu-id="24ec8-132">Music</span><span class="sxs-lookup"><span data-stu-id="24ec8-132">Music</span></span>       | `music`      | <span data-ttu-id="24ec8-p106">ミュージック フォルダーです。OneDrive for Business では利用不可です。</span><span class="sxs-lookup"><span data-stu-id="24ec8-p106">The Music folder. Not available in OneDrive for Business.</span></span>                |
| <span data-ttu-id="24ec8-135">Photos</span><span class="sxs-lookup"><span data-stu-id="24ec8-135">Photos</span></span>      | `photos`     | <span data-ttu-id="24ec8-136">フォト フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="24ec8-136">The Photos folder.</span></span>                                                       |

## <a name="remarks"></a><span data-ttu-id="24ec8-137">備考</span><span class="sxs-lookup"><span data-stu-id="24ec8-137">Remarks</span></span> 

<span data-ttu-id="24ec8-138">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24ec8-138">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
