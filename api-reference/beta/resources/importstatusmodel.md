---
title: importStatusModel リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: 8174594d819803ddfe6a23e69be170bb2fdda912
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069574"
---
# <a name="importstatusmodel-resource-type"></a><span data-ttu-id="644b8-103">importStatusModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="644b8-103">importStatusModel resource type</span></span>

> <span data-ttu-id="644b8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="644b8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="644b8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="644b8-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="644b8-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="644b8-106">JSON representation</span></span>

<span data-ttu-id="644b8-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="644b8-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.importstatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="644b8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644b8-108">Properties</span></span>
| <span data-ttu-id="644b8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644b8-109">Property</span></span>     | <span data-ttu-id="644b8-110">型</span><span class="sxs-lookup"><span data-stu-id="644b8-110">Type</span></span>   |<span data-ttu-id="644b8-111">説明</span><span class="sxs-lookup"><span data-stu-id="644b8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="644b8-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="644b8-112">createdDateTime</span></span>| <span data-ttu-id="644b8-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="644b8-113">DateTimeOffset</span></span> ||
|<span data-ttu-id="644b8-114">ID</span><span class="sxs-lookup"><span data-stu-id="644b8-114">id</span></span>|<span data-ttu-id="644b8-115">文字列</span><span class="sxs-lookup"><span data-stu-id="644b8-115">string</span></span>||
|<span data-ttu-id="644b8-116">status</span><span class="sxs-lookup"><span data-stu-id="644b8-116">status</span></span>|<span data-ttu-id="644b8-117">文字列</span><span class="sxs-lookup"><span data-stu-id="644b8-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "importStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
