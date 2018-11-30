---
title: copyStatusModel リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: 8a4726715885e46208183aebe093f388a308de01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066767"
---
# <a name="copystatusmodel-resource-type"></a><span data-ttu-id="31174-103">copyStatusModel リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31174-103">copyStatusModel resource type</span></span>

> <span data-ttu-id="31174-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31174-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31174-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31174-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31174-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31174-106">JSON representation</span></span>

<span data-ttu-id="31174-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="31174-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.copystatusmodel"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "id": "string",
  "status": "string"
}

```
## <a name="properties"></a><span data-ttu-id="31174-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31174-108">Properties</span></span>
| <span data-ttu-id="31174-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31174-109">Property</span></span>     | <span data-ttu-id="31174-110">型</span><span class="sxs-lookup"><span data-stu-id="31174-110">Type</span></span>   |<span data-ttu-id="31174-111">説明</span><span class="sxs-lookup"><span data-stu-id="31174-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31174-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31174-112">createdDateTime</span></span>| <span data-ttu-id="31174-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31174-113">DateTimeOffset</span></span> ||
|<span data-ttu-id="31174-114">ID</span><span class="sxs-lookup"><span data-stu-id="31174-114">id</span></span>|<span data-ttu-id="31174-115">文字列</span><span class="sxs-lookup"><span data-stu-id="31174-115">string</span></span>||
|<span data-ttu-id="31174-116">status</span><span class="sxs-lookup"><span data-stu-id="31174-116">status</span></span>|<span data-ttu-id="31174-117">文字列</span><span class="sxs-lookup"><span data-stu-id="31174-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "copyStatusModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
