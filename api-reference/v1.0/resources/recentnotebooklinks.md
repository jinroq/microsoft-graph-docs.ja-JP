---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くためのリンクです。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f112d8ff87329ca23a3a44fb33dafe4582072519
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034833"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="8494f-104">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="8494f-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="8494f-105">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="8494f-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="8494f-106">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="8494f-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="8494f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8494f-107">Properties</span></span>
| <span data-ttu-id="8494f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8494f-108">Property</span></span>     | <span data-ttu-id="8494f-109">型</span><span class="sxs-lookup"><span data-stu-id="8494f-109">Type</span></span>   |<span data-ttu-id="8494f-110">説明</span><span class="sxs-lookup"><span data-stu-id="8494f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8494f-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="8494f-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="8494f-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="8494f-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="8494f-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="8494f-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="8494f-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="8494f-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="8494f-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="8494f-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="8494f-116">OneNote で web 上のノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="8494f-116">Opens the notebook in OneNote on the web.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8494f-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8494f-117">JSON representation</span></span>

<span data-ttu-id="8494f-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8494f-118">The following is a JSON representation of the resource.</span></span>

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
