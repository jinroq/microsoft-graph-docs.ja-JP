---
author: JeremyKelley
ms.author: jeremyke
title: アルバムリソースの種類
description: フォトアルバムであるバンドルを記述するファセット。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3bb5391557c3dfb0a97702a0e78de60c0a4876c7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932878"
---
# <a name="album-resource-type"></a><span data-ttu-id="d10ef-103">アルバムリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d10ef-103">album resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d10ef-104">フォトアルバムは、1つの[バンドル][]内で、ハードファセット[][]を使用して、事実上グループ化された[ドライブ][]アイテムをグループ化する方法です。</span><span class="sxs-lookup"><span data-stu-id="d10ef-104">A photo album is a way to virtually group [driveItems][driveItem] with [photo][] facets together in a [bundle][].</span></span> <span data-ttu-id="d10ef-105">このタイプのバンドルには、[バンドル][]リソースに**アルバム**プロパティが設定されます。</span><span class="sxs-lookup"><span data-stu-id="d10ef-105">Bundles of this type will have the **album** property set on the [bundle][] resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d10ef-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d10ef-106">Properties</span></span>

| <span data-ttu-id="d10ef-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="d10ef-107">Property name</span></span>     | <span data-ttu-id="d10ef-108">種類</span><span class="sxs-lookup"><span data-stu-id="d10ef-108">Type</span></span>   | <span data-ttu-id="d10ef-109">説明</span><span class="sxs-lookup"><span data-stu-id="d10ef-109">Description</span></span>
|:------------------|:-------|:------------------------------------------------
| <span data-ttu-id="d10ef-110">イメージ Itemid のカバー</span><span class="sxs-lookup"><span data-stu-id="d10ef-110">coverImageItemId</span></span> | <span data-ttu-id="d10ef-111">String</span><span class="sxs-lookup"><span data-stu-id="d10ef-111">String</span></span> | <span data-ttu-id="d10ef-112">アルバムのカバーである[ドライブ項目][]の一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="d10ef-112">Unique identifier of the [driveItem][] that is the cover of the album.</span></span>

<span data-ttu-id="d10ef-113">**注:** カバーされていない**Imageitemid**が前に設定されていない場合は、アルバムのサムネイルが自動的に選択されます。</span><span class="sxs-lookup"><span data-stu-id="d10ef-113">**Note:** If a **coverImageItemId** has not been set before, the thumbnails for an album are chosen automatically.</span></span>
<span data-ttu-id="d10ef-114">**イメージ itemid**が設定された後は、アルバムのサムネイルは常にその id に関連付けられているアイテムになります。[バンドルアイテム][バンドル]にパッチを適用し、の`album`カバー **imageitemid**プロパティをアルバム内に含まれる画像の id に設定することで、既定のカバーを上書きできます。</span><span class="sxs-lookup"><span data-stu-id="d10ef-114">After **coverImageItemId** has been set, the thumbnails for an album will always be the item associated with that id. You can override the default cover by PATCHing the [bundle item][bundle] and setting the **coverImageItemId** property on the `album` to the id of an image contained within the album.</span></span>
<span data-ttu-id="d10ef-115">ユーザー設定の表紙を削除するには、カバー **Imageitemid**プロパティを null に設定し、既定値を自動的に選択します。</span><span class="sxs-lookup"><span data-stu-id="d10ef-115">To remove a custom-set cover, you can set the **coverImageItemId** property to null, and a default one will be chosen automatically again.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d10ef-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d10ef-116">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[バンドル]: bundle.md
[bundle]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
