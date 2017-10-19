---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: ee869e5f2925af92fea9eef04fd26ec483baad5b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="ca8a4-102">ContentType リソース型</span><span class="sxs-lookup"><span data-stu-id="ca8a4-102">ContentType resource type</span></span>

<span data-ttu-id="ca8a4-103">**contentType** リソースは、SharePoint の_コンテンツ タイプ_を表します。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-103">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="ca8a4-104">コンテンツ タイプによって、[**list**][list] 内の [**listItem**][listItem] ごとに存在する必要のある列のセットを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-104">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listItem.md

## <a name="json-representation"></a><span data-ttu-id="ca8a4-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca8a4-105">JSON representation</span></span>

<span data-ttu-id="ca8a4-106">以下は、**contentType** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-106">Here is a JSON representation of a **baseItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

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

## <a name="properties"></a><span data-ttu-id="ca8a4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca8a4-107">Properties</span></span>

| <span data-ttu-id="ca8a4-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ca8a4-108">Property name</span></span>     | <span data-ttu-id="ca8a4-109">種類</span><span class="sxs-lookup"><span data-stu-id="ca8a4-109">Type</span></span>                 | <span data-ttu-id="ca8a4-110">説明</span><span class="sxs-lookup"><span data-stu-id="ca8a4-110">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="ca8a4-111">**description**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-111">**description**</span></span>   | <span data-ttu-id="ca8a4-112">string</span><span class="sxs-lookup"><span data-stu-id="ca8a4-112">string</span></span>               | <span data-ttu-id="ca8a4-113">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-113">The descriptive text for the site.</span></span>
| <span data-ttu-id="ca8a4-114">**group**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-114">**group**</span></span>         | <span data-ttu-id="ca8a4-115">string</span><span class="sxs-lookup"><span data-stu-id="ca8a4-115">string</span></span>               | <span data-ttu-id="ca8a4-116">このコンテンツ タイプが属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-116">The name of the group this content type belongs to.</span></span> <span data-ttu-id="ca8a4-117">関連するコンテンツ タイプを整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-117">Helps organize related content types.</span></span>
| <span data-ttu-id="ca8a4-118">**hidden**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-118">**hidden**</span></span>        | <span data-ttu-id="ca8a4-119">boolean</span><span class="sxs-lookup"><span data-stu-id="ca8a4-119">boolean</span></span>              | <span data-ttu-id="ca8a4-120">コンテンツ タイプがリストの [新規作成] メニューで非表示かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-120">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="ca8a4-121">**id**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-121">**id**</span></span>            | <span data-ttu-id="ca8a4-122">string</span><span class="sxs-lookup"><span data-stu-id="ca8a4-122">string</span></span>               | <span data-ttu-id="ca8a4-123">コンテンツ タイプの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-123">The unique identifier of the content type.</span></span>
| <span data-ttu-id="ca8a4-124">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-124">**inheritedFrom**</span></span> | <span data-ttu-id="ca8a4-125">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="ca8a4-125">[itemReference][]</span></span>    | <span data-ttu-id="ca8a4-126">このコンテンツ タイプが、別のスコープ (サイトなど) から継承されている場合、そのコンテンツ タイプが定義されているアイテムへの参照を提供します。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-126">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="ca8a4-127">**name**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-127">**name**</span></span>          | <span data-ttu-id="ca8a4-128">string</span><span class="sxs-lookup"><span data-stu-id="ca8a4-128">string</span></span>               | <span data-ttu-id="ca8a4-129">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-129">The name of the content type.</span></span>
| <span data-ttu-id="ca8a4-130">**order**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-130">**order**</span></span>         | <span data-ttu-id="ca8a4-131">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="ca8a4-131">[contentTypeOrder][]</span></span> | <span data-ttu-id="ca8a4-132">選択 UI でコンテンツ タイプを表示する順番を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-132">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="ca8a4-133">**parentId**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-133">**ParentId**</span></span>      | <span data-ttu-id="ca8a4-134">string</span><span class="sxs-lookup"><span data-stu-id="ca8a4-134">string</span></span>               | <span data-ttu-id="ca8a4-135">コンテンツ タイプの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-135">The unique identifier of the content type.</span></span>
| <span data-ttu-id="ca8a4-136">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-136">**Read-only.**</span></span>      | <span data-ttu-id="ca8a4-137">boolean</span><span class="sxs-lookup"><span data-stu-id="ca8a4-137">boolean</span></span>              | <span data-ttu-id="ca8a4-138">`true` の場合、コンテンツ タイプは変更できません。変更する場合は、この値を先に `false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-138">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="ca8a4-139">**sealed**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-139">**sealed**</span></span>        | <span data-ttu-id="ca8a4-140">boolean</span><span class="sxs-lookup"><span data-stu-id="ca8a4-140">boolean</span></span>              | <span data-ttu-id="ca8a4-141">`true` の場合、ユーザーまたはプッシュダウン操作ではコンテンツ タイプを変更できません。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-141">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="ca8a4-142">サイト コレクションの管理者だけがコンテンツ タイプのシールまたはシール解除ができます。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-142">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="ca8a4-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ca8a4-143">Relationships</span></span>

| <span data-ttu-id="ca8a4-144">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ca8a4-144">Property name</span></span>   | <span data-ttu-id="ca8a4-145">種類</span><span class="sxs-lookup"><span data-stu-id="ca8a4-145">Type</span></span>                      | <span data-ttu-id="ca8a4-146">説明</span><span class="sxs-lookup"><span data-stu-id="ca8a4-146">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="ca8a4-147">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="ca8a4-147">**columnLinks**</span></span> | <span data-ttu-id="ca8a4-148">[columnLink][] コレクション</span><span class="sxs-lookup"><span data-stu-id="ca8a4-148">[columnLink][] collection</span></span> | <span data-ttu-id="ca8a4-149">このコンテンツ タイプに必要とされる列のコレクション</span><span class="sxs-lookup"><span data-stu-id="ca8a4-149">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="ca8a4-150">詳細については、「[コンテンツ タイプとコンテンツ タイプ発行の概要][contentTypeIntro]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca8a4-150">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
