---
title: 拡張子リソースの種類
description: OData v4 のオープン型 openTypeExtension をサポートする抽象型。
localization_priority: Normal
ms.openlocfilehash: b261ceeff4639b8a602edbb411b34ab19d46ea8e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542637"
---
# <a name="extension-resource-type"></a><span data-ttu-id="b4870-103">拡張子リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4870-103">extension resource type</span></span>

<span data-ttu-id="b4870-104">OData v4 のオープン型 [openTypeExtension](opentypeextension.md) をサポートする抽象型。</span><span class="sxs-lookup"><span data-stu-id="b4870-104">An abstract type to support the OData v4 open type [openTypeExtension](opentypeextension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4870-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4870-105">JSON representation</span></span>

<span data-ttu-id="b4870-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b4870-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="b4870-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4870-107">Properties</span></span>
| <span data-ttu-id="b4870-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4870-108">Property</span></span>     | <span data-ttu-id="b4870-109">型</span><span class="sxs-lookup"><span data-stu-id="b4870-109">Type</span></span>   |<span data-ttu-id="b4870-110">説明</span><span class="sxs-lookup"><span data-stu-id="b4870-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4870-111">id</span><span class="sxs-lookup"><span data-stu-id="b4870-111">id</span></span>|<span data-ttu-id="b4870-112">String</span><span class="sxs-lookup"><span data-stu-id="b4870-112">String</span></span>| <span data-ttu-id="b4870-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4870-113">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4870-114">関係</span><span class="sxs-lookup"><span data-stu-id="b4870-114">Relationships</span></span>
<span data-ttu-id="b4870-115">なし</span><span class="sxs-lookup"><span data-stu-id="b4870-115">None</span></span>


## <a name="methods"></a><span data-ttu-id="b4870-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="b4870-116">Methods</span></span>

<span data-ttu-id="b4870-117">実際にサポートされるメソッドについては、派生型「[openTypeExtension](opentypeextension.md)」のメソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4870-117">See the methods of the derived type [openTypeExtension](opentypeextension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
