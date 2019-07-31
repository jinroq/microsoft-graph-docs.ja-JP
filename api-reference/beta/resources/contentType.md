---
author: daspek
description: contentType リソースは、SharePoint のコンテンツ タイプを表します。
ms.date: 09/12/2017
title: ContentType
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7376b431154595f9b3d2de1931918b629e74acb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012864"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="b57ae-103">ContentType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b57ae-103">ContentType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b57ae-104">**contentType** リソースは、SharePoint の_コンテンツ タイプ_を表します。</span><span class="sxs-lookup"><span data-stu-id="b57ae-104">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="b57ae-105">コンテンツタイプを使用すると、[**リスト**][list]内のすべての[**listItem**][listItem]に存在する必要がある列のセットを定義できます。</span><span class="sxs-lookup"><span data-stu-id="b57ae-105">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="b57ae-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b57ae-106">JSON representation</span></span>

<span data-ttu-id="b57ae-107">以下は、**contentType** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b57ae-107">Here is a JSON representation of a **contentType** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType","keyProperty":"id" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a><span data-ttu-id="b57ae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b57ae-108">Properties</span></span>

| <span data-ttu-id="b57ae-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b57ae-109">Property name</span></span>     | <span data-ttu-id="b57ae-110">種類</span><span class="sxs-lookup"><span data-stu-id="b57ae-110">Type</span></span>                 | <span data-ttu-id="b57ae-111">説明</span><span class="sxs-lookup"><span data-stu-id="b57ae-111">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="b57ae-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b57ae-112">**description**</span></span>   | <span data-ttu-id="b57ae-113">string</span><span class="sxs-lookup"><span data-stu-id="b57ae-113">string</span></span>               | <span data-ttu-id="b57ae-114">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="b57ae-114">The descriptive text for the item.</span></span>
| <span data-ttu-id="b57ae-115">**group**</span><span class="sxs-lookup"><span data-stu-id="b57ae-115">**group**</span></span>         | <span data-ttu-id="b57ae-116">string</span><span class="sxs-lookup"><span data-stu-id="b57ae-116">string</span></span>               | <span data-ttu-id="b57ae-117">このコンテンツ タイプが属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="b57ae-117">The name of the group this content type belongs to.</span></span> <span data-ttu-id="b57ae-118">関連するコンテンツ タイプを整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="b57ae-118">Helps organize related content types.</span></span>
| <span data-ttu-id="b57ae-119">**hidden**</span><span class="sxs-lookup"><span data-stu-id="b57ae-119">**hidden**</span></span>        | <span data-ttu-id="b57ae-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="b57ae-120">boolean</span></span>              | <span data-ttu-id="b57ae-121">コンテンツ タイプがリストの [新規作成] メニューで非表示かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b57ae-121">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="b57ae-122">**id**</span><span class="sxs-lookup"><span data-stu-id="b57ae-122">**id**</span></span>            | <span data-ttu-id="b57ae-123">string</span><span class="sxs-lookup"><span data-stu-id="b57ae-123">string</span></span>               | <span data-ttu-id="b57ae-124">コンテンツ タイプの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b57ae-124">The unique identifier of the content type.</span></span>
| <span data-ttu-id="b57ae-125">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="b57ae-125">**inheritedFrom**</span></span> | <span data-ttu-id="b57ae-126">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="b57ae-126">[itemReference][]</span></span>    | <span data-ttu-id="b57ae-127">このコンテンツ タイプが、別のスコープ (サイトなど) から継承されている場合、そのコンテンツ タイプが定義されているアイテムへの参照を提供します。</span><span class="sxs-lookup"><span data-stu-id="b57ae-127">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="b57ae-128">**name**</span><span class="sxs-lookup"><span data-stu-id="b57ae-128">**name**</span></span>          | <span data-ttu-id="b57ae-129">string</span><span class="sxs-lookup"><span data-stu-id="b57ae-129">string</span></span>               | <span data-ttu-id="b57ae-130">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="b57ae-130">The name of the content type.</span></span>
| <span data-ttu-id="b57ae-131">**order**</span><span class="sxs-lookup"><span data-stu-id="b57ae-131">**order**</span></span>         | <span data-ttu-id="b57ae-132">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="b57ae-132">[contentTypeOrder][]</span></span> | <span data-ttu-id="b57ae-133">選択 UI でコンテンツ タイプを表示する順番を指定します。</span><span class="sxs-lookup"><span data-stu-id="b57ae-133">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="b57ae-134">**parentId**</span><span class="sxs-lookup"><span data-stu-id="b57ae-134">**parentId**</span></span>      | <span data-ttu-id="b57ae-135">string</span><span class="sxs-lookup"><span data-stu-id="b57ae-135">string</span></span>               | <span data-ttu-id="b57ae-136">コンテンツ タイプの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b57ae-136">The unique identifier of the content type.</span></span>
| <span data-ttu-id="b57ae-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="b57ae-137">**readOnly**</span></span>      | <span data-ttu-id="b57ae-138">ブール値</span><span class="sxs-lookup"><span data-stu-id="b57ae-138">boolean</span></span>              | <span data-ttu-id="b57ae-139">`true` である場合、コンテンツ タイプは変更できません。変更する場合は、この値を先に `false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="b57ae-139">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="b57ae-140">**sealed**</span><span class="sxs-lookup"><span data-stu-id="b57ae-140">**sealed**</span></span>        | <span data-ttu-id="b57ae-141">boolean</span><span class="sxs-lookup"><span data-stu-id="b57ae-141">boolean</span></span>              | <span data-ttu-id="b57ae-142">`true` である場合、ユーザーまたはプッシュダウン操作ではコンテンツ タイプを変更できません。</span><span class="sxs-lookup"><span data-stu-id="b57ae-142">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="b57ae-143">サイト コレクションの管理者だけがコンテンツ タイプのシールまたはシール解除ができます。</span><span class="sxs-lookup"><span data-stu-id="b57ae-143">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="b57ae-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b57ae-144">Relationships</span></span>

| <span data-ttu-id="b57ae-145">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b57ae-145">Property name</span></span>   | <span data-ttu-id="b57ae-146">種類</span><span class="sxs-lookup"><span data-stu-id="b57ae-146">Type</span></span>                      | <span data-ttu-id="b57ae-147">説明</span><span class="sxs-lookup"><span data-stu-id="b57ae-147">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="b57ae-148">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="b57ae-148">**columnLinks**</span></span> | <span data-ttu-id="b57ae-149">[columnLink][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b57ae-149">[columnLink][] collection</span></span> | <span data-ttu-id="b57ae-150">このコンテンツ タイプに必要とされる列のコレクション</span><span class="sxs-lookup"><span data-stu-id="b57ae-150">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="b57ae-151">詳細については、「[コンテンツ タイプとコンテンツ タイプ発行の概要][contentTypeIntro]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b57ae-151">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType",
  "suppressions": []
}
-->
