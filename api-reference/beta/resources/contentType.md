---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: cda50c2f20df14c733d3bf71e1b84d5b0df225a0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072944"
---
# <a name="contenttype-resource-type"></a><span data-ttu-id="e289b-102">ContentType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e289b-102">ContentType resource type</span></span>

> <span data-ttu-id="e289b-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e289b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e289b-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e289b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e289b-105">**contentType** リソースは、SharePoint の_コンテンツ タイプ_を表します。</span><span class="sxs-lookup"><span data-stu-id="e289b-105">The **contentType** resource represents a _content type_ in SharePoint.</span></span>
<span data-ttu-id="e289b-106">コンテンツ タイプによって、[**list**][list] 内のすべての [**listItem**][listItem] に存在する必要のある列のセットを定義することができます。</span><span class="sxs-lookup"><span data-stu-id="e289b-106">Content types allow you to define a set of columns that must be present on every [**listItem**][listItem] in a [**list**][list].</span></span>

[list]: list.md
[listItem]: listitem.md

## <a name="json-representation"></a><span data-ttu-id="e289b-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e289b-107">JSON representation</span></span>

<span data-ttu-id="e289b-108">以下は、**contentType** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e289b-108">Here is a JSON representation of a **contentType** resource.</span></span>
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

## <a name="properties"></a><span data-ttu-id="e289b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e289b-109">Properties</span></span>

| <span data-ttu-id="e289b-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e289b-110">Property name</span></span>     | <span data-ttu-id="e289b-111">型</span><span class="sxs-lookup"><span data-stu-id="e289b-111">Type</span></span>                 | <span data-ttu-id="e289b-112">説明</span><span class="sxs-lookup"><span data-stu-id="e289b-112">Description</span></span>
|:------------------|:---------------------|:----------------------------------
| <span data-ttu-id="e289b-113">**description**</span><span class="sxs-lookup"><span data-stu-id="e289b-113">**description**</span></span>   | <span data-ttu-id="e289b-114">文字列</span><span class="sxs-lookup"><span data-stu-id="e289b-114">string</span></span>               | <span data-ttu-id="e289b-115">アイテムの説明テキストです。</span><span class="sxs-lookup"><span data-stu-id="e289b-115">The descriptive text for the item.</span></span>
| <span data-ttu-id="e289b-116">**group**</span><span class="sxs-lookup"><span data-stu-id="e289b-116">**group**</span></span>         | <span data-ttu-id="e289b-117">文字列</span><span class="sxs-lookup"><span data-stu-id="e289b-117">string</span></span>               | <span data-ttu-id="e289b-118">このコンテンツ タイプが属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="e289b-118">The name of the group this content type belongs to.</span></span> <span data-ttu-id="e289b-119">関連するコンテンツ タイプを整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e289b-119">Helps organize related content types.</span></span>
| <span data-ttu-id="e289b-120">**hidden**</span><span class="sxs-lookup"><span data-stu-id="e289b-120">**hidden**</span></span>        | <span data-ttu-id="e289b-121">boolean</span><span class="sxs-lookup"><span data-stu-id="e289b-121">boolean</span></span>              | <span data-ttu-id="e289b-122">コンテンツ タイプがリストの [新規作成] メニューで非表示かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e289b-122">Indicates whether the content type is hidden in the list's 'New' menu.</span></span>
| <span data-ttu-id="e289b-123">**id**</span><span class="sxs-lookup"><span data-stu-id="e289b-123">**id**</span></span>            | <span data-ttu-id="e289b-124">string</span><span class="sxs-lookup"><span data-stu-id="e289b-124">string</span></span>               | <span data-ttu-id="e289b-125">コンテンツ タイプの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e289b-125">The unique identifier of the content type.</span></span>
| <span data-ttu-id="e289b-126">**inheritedFrom**</span><span class="sxs-lookup"><span data-stu-id="e289b-126">**inheritedFrom**</span></span> | <span data-ttu-id="e289b-127">[itemReference][]</span><span class="sxs-lookup"><span data-stu-id="e289b-127">[itemReference][]</span></span>    | <span data-ttu-id="e289b-128">このコンテンツ タイプが、別のスコープ (サイトなど) から継承されている場合、そのコンテンツ タイプが定義されているアイテムへの参照を提供します。</span><span class="sxs-lookup"><span data-stu-id="e289b-128">If this content type is inherited from another scope (like a site), provides a reference to the item where the content type is defined.</span></span>
| <span data-ttu-id="e289b-129">**name**</span><span class="sxs-lookup"><span data-stu-id="e289b-129">**name**</span></span>          | <span data-ttu-id="e289b-130">文字列</span><span class="sxs-lookup"><span data-stu-id="e289b-130">string</span></span>               | <span data-ttu-id="e289b-131">コンテンツ タイプの名前。</span><span class="sxs-lookup"><span data-stu-id="e289b-131">The name of the content type.</span></span>
| <span data-ttu-id="e289b-132">**order**</span><span class="sxs-lookup"><span data-stu-id="e289b-132">**order**</span></span>         | <span data-ttu-id="e289b-133">[contentTypeOrder][]</span><span class="sxs-lookup"><span data-stu-id="e289b-133">[contentTypeOrder][]</span></span> | <span data-ttu-id="e289b-134">選択 UI でコンテンツ タイプを表示する順番を指定します。</span><span class="sxs-lookup"><span data-stu-id="e289b-134">Specifies the order in which the content type appears in the selection UI.</span></span>
| <span data-ttu-id="e289b-135">**parentId**</span><span class="sxs-lookup"><span data-stu-id="e289b-135">**parentId**</span></span>      | <span data-ttu-id="e289b-136">文字列</span><span class="sxs-lookup"><span data-stu-id="e289b-136">string</span></span>               | <span data-ttu-id="e289b-137">コンテンツ タイプの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e289b-137">The unique identifier of the content type.</span></span>
| <span data-ttu-id="e289b-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="e289b-138">**readOnly**</span></span>      | <span data-ttu-id="e289b-139">boolean</span><span class="sxs-lookup"><span data-stu-id="e289b-139">boolean</span></span>              | <span data-ttu-id="e289b-140">`true` である場合、コンテンツ タイプは変更できません。変更する場合は、この値を先に `false` に設定します。</span><span class="sxs-lookup"><span data-stu-id="e289b-140">If `true`, the content type cannot be modified unless this value is first set to `false`.</span></span>
| <span data-ttu-id="e289b-141">**sealed**</span><span class="sxs-lookup"><span data-stu-id="e289b-141">**sealed**</span></span>        | <span data-ttu-id="e289b-142">boolean</span><span class="sxs-lookup"><span data-stu-id="e289b-142">boolean</span></span>              | <span data-ttu-id="e289b-143">`true` である場合、ユーザーまたはプッシュダウン操作ではコンテンツ タイプを変更できません。</span><span class="sxs-lookup"><span data-stu-id="e289b-143">If `true`, the content type cannot be modified by users or through push-down operations.</span></span> <span data-ttu-id="e289b-144">サイト コレクションの管理者だけがコンテンツ タイプのシールまたはシール解除ができます。</span><span class="sxs-lookup"><span data-stu-id="e289b-144">Only site collection administrators can seal or unseal content types.</span></span>

## <a name="relationships"></a><span data-ttu-id="e289b-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e289b-145">Relationships</span></span>

| <span data-ttu-id="e289b-146">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e289b-146">Property name</span></span>   | <span data-ttu-id="e289b-147">型</span><span class="sxs-lookup"><span data-stu-id="e289b-147">Type</span></span>                      | <span data-ttu-id="e289b-148">説明</span><span class="sxs-lookup"><span data-stu-id="e289b-148">Description</span></span>
|:----------------|:--------------------------|:-------------------------------
| <span data-ttu-id="e289b-149">**columnLinks**</span><span class="sxs-lookup"><span data-stu-id="e289b-149">**columnLinks**</span></span> | <span data-ttu-id="e289b-150">[columnLink][] コレクション</span><span class="sxs-lookup"><span data-stu-id="e289b-150">[columnLink][] collection</span></span> | <span data-ttu-id="e289b-151">このコンテンツ タイプに必要とされる列のコレクション</span><span class="sxs-lookup"><span data-stu-id="e289b-151">The collection of columns that are required by this content type</span></span>

<span data-ttu-id="e289b-152">詳細については、「[コンテンツ タイプとコンテンツ タイプ発行の概要][contentTypeIntro]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e289b-152">See [Introduction to content types and content type publishing][contentTypeIntro] for more information.</span></span>

[columnLink]: columnlink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemreference.md
[contentTypeOrder]: contenttypeorder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
