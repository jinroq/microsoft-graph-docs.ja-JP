---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
ms.openlocfilehash: b67c347e44c875ca550465be46eecdff3f845eef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067519"
---
# <a name="extension-resource-type"></a><span data-ttu-id="32680-103">拡張子リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32680-103">extension resource type</span></span>

> <span data-ttu-id="32680-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32680-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32680-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32680-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32680-106">OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。</span><span class="sxs-lookup"><span data-stu-id="32680-106">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="32680-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32680-107">JSON representation</span></span>

<span data-ttu-id="32680-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="32680-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="32680-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32680-109">Properties</span></span>
| <span data-ttu-id="32680-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32680-110">Property</span></span>     | <span data-ttu-id="32680-111">型</span><span class="sxs-lookup"><span data-stu-id="32680-111">Type</span></span>   |<span data-ttu-id="32680-112">説明</span><span class="sxs-lookup"><span data-stu-id="32680-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32680-113">id</span><span class="sxs-lookup"><span data-stu-id="32680-113">id</span></span>|<span data-ttu-id="32680-114">String</span><span class="sxs-lookup"><span data-stu-id="32680-114">String</span></span>| <span data-ttu-id="32680-115">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="32680-115">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32680-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32680-116">Relationships</span></span>
<span data-ttu-id="32680-117">なし</span><span class="sxs-lookup"><span data-stu-id="32680-117">None</span></span>


## <a name="methods"></a><span data-ttu-id="32680-118">メソッド</span><span class="sxs-lookup"><span data-stu-id="32680-118">Methods</span></span>

<span data-ttu-id="32680-119">実際にサポートされるメソッドについては、派生型「[openTypeExtension](opentypeextension.md)」のメソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="32680-119">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->