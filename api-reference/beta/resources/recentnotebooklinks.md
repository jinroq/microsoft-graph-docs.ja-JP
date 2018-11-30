---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くへのリンクです。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
ms.openlocfilehash: de13f25148425a1816a60f6cf5b9f4a09f61c7dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070062"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="19f1d-104">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="19f1d-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="19f1d-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19f1d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19f1d-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19f1d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19f1d-107">OneNote ノートブックを開くへのリンクです。</span><span class="sxs-lookup"><span data-stu-id="19f1d-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="19f1d-108">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="19f1d-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="19f1d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19f1d-109">Properties</span></span>
| <span data-ttu-id="19f1d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19f1d-110">Property</span></span>     | <span data-ttu-id="19f1d-111">型</span><span class="sxs-lookup"><span data-stu-id="19f1d-111">Type</span></span>   |<span data-ttu-id="19f1d-112">説明</span><span class="sxs-lookup"><span data-stu-id="19f1d-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19f1d-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="19f1d-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="19f1d-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="19f1d-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="19f1d-115">インストールされている場合は、OneNote クライアントで、ノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="19f1d-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="19f1d-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="19f1d-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="19f1d-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="19f1d-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="19f1d-118">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="19f1d-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="19f1d-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19f1d-119">JSON representation</span></span>

<span data-ttu-id="19f1d-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="19f1d-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
