---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Folder
ms.openlocfilehash: 834b2cd7c81a947ca1e6d4619f39a8533677e6c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072539"
---
# <a name="folder-resource-type"></a><span data-ttu-id="78a9c-102">Folder リソース型</span><span class="sxs-lookup"><span data-stu-id="78a9c-102">Folder resource type</span></span>

> <span data-ttu-id="78a9c-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78a9c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78a9c-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78a9c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78a9c-p102">**フォルダー**リソースは、アイテム上のフォルダー関連のデータを 1 つの構造にグループ化します。**フォルダー**ファセットが null 以外の [**DriveItems**](driveitem.md) は、他の DriveItems のコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="78a9c-p102">The **Folder** resource groups folder-related data on an item into a single structure. [**DriveItems**](driveitem.md) with a non-null **folder** facet are containers for other DriveItems.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78a9c-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78a9c-107">JSON representation</span></span>

<span data-ttu-id="78a9c-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78a9c-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.folder"
}-->

```json
{
  "childCount": 1024,
  "view": { "@odata.type": "microsoft.graph.folderView" }
}
```

## <a name="properties"></a><span data-ttu-id="78a9c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78a9c-109">Properties</span></span>

| <span data-ttu-id="78a9c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78a9c-110">Property</span></span>       | <span data-ttu-id="78a9c-111">型</span><span class="sxs-lookup"><span data-stu-id="78a9c-111">Type</span></span>           | <span data-ttu-id="78a9c-112">説明</span><span class="sxs-lookup"><span data-stu-id="78a9c-112">Description</span></span>
|:---------------|:---------------|:-------------------------------------------
| <span data-ttu-id="78a9c-113">**childCount**</span><span class="sxs-lookup"><span data-stu-id="78a9c-113">**childCount**</span></span> | <span data-ttu-id="78a9c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="78a9c-114">Int64</span></span>          | <span data-ttu-id="78a9c-115">このコンテナーの中に含まれる子の数。</span><span class="sxs-lookup"><span data-stu-id="78a9c-115">Number of children contained immediately within this container.</span></span>
| <span data-ttu-id="78a9c-116">**view**</span><span class="sxs-lookup"><span data-stu-id="78a9c-116">**view**</span></span>       | <span data-ttu-id="78a9c-117">[folderView][]</span><span class="sxs-lookup"><span data-stu-id="78a9c-117">[folderView][]</span></span> | <span data-ttu-id="78a9c-118">フォルダーに推奨されるビューを定義するプロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="78a9c-118">A collection of properties defining the recommended view for the folder.</span></span>


## <a name="remarks"></a><span data-ttu-id="78a9c-119">備考</span><span class="sxs-lookup"><span data-stu-id="78a9c-119">Remarks</span></span> 

<span data-ttu-id="78a9c-120">DriveItem のファセットの詳細については、「[DriveItem][]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78a9c-120">For more information about the facets on a DriveItem, see [DriveItem][].</span></span>

[folderView]: folderview.md
[DriveItem]: driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "folder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
