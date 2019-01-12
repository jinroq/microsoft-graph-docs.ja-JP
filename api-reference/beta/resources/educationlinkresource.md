---
title: educationLinkResource リソースの種類
description: EducationResource のサブクラスです。 このリソースは、リンクとは必要なデータに関連付けられていないことです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8cdcb47c02481f2f43ee71f46c24e2b8d8f5ba2a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918050"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="1f18f-104">educationLinkResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1f18f-104">educationLinkResource resource type</span></span>

> <span data-ttu-id="1f18f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f18f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f18f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f18f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1f18f-107">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="1f18f-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="1f18f-108">このリソースは、リンクとは必要なデータに関連付けられていないことです。</span><span class="sxs-lookup"><span data-stu-id="1f18f-108">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="1f18f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f18f-109">Properties</span></span>
| <span data-ttu-id="1f18f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f18f-110">Property</span></span>     | <span data-ttu-id="1f18f-111">種類</span><span class="sxs-lookup"><span data-stu-id="1f18f-111">Type</span></span>   |<span data-ttu-id="1f18f-112">説明</span><span class="sxs-lookup"><span data-stu-id="1f18f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f18f-113">link</span><span class="sxs-lookup"><span data-stu-id="1f18f-113">link</span></span>|<span data-ttu-id="1f18f-114">String</span><span class="sxs-lookup"><span data-stu-id="1f18f-114">String</span></span>|<span data-ttu-id="1f18f-115">リソースへの URL です。</span><span class="sxs-lookup"><span data-stu-id="1f18f-115">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f18f-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f18f-116">JSON representation</span></span>

<span data-ttu-id="1f18f-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f18f-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
