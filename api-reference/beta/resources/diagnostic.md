---
title: 診断リソースの種類
description: OneNote の操作に関するエラーまたは警告に関する情報。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4ac591640e647a1caa5230bd8e7e8c64ad2314af
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973149"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="b5e57-103">診断リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5e57-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e57-104">OneNote の操作に関するエラーまたは警告に関する情報。</span><span class="sxs-lookup"><span data-stu-id="b5e57-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5e57-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5e57-105">JSON representation</span></span>

<span data-ttu-id="b5e57-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b5e57-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="b5e57-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5e57-107">Properties</span></span>
| <span data-ttu-id="b5e57-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5e57-108">Property</span></span>     | <span data-ttu-id="b5e57-109">型</span><span class="sxs-lookup"><span data-stu-id="b5e57-109">Type</span></span>   |<span data-ttu-id="b5e57-110">説明</span><span class="sxs-lookup"><span data-stu-id="b5e57-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5e57-111">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="b5e57-111">message</span></span>|<span data-ttu-id="b5e57-112">String</span><span class="sxs-lookup"><span data-stu-id="b5e57-112">String</span></span>|<span data-ttu-id="b5e57-113">エラーまたは警告を発生させた条件を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="b5e57-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="b5e57-114">url</span><span class="sxs-lookup"><span data-stu-id="b5e57-114">url</span></span>|<span data-ttu-id="b5e57-115">String</span><span class="sxs-lookup"><span data-stu-id="b5e57-115">String</span></span>|<span data-ttu-id="b5e57-116">この問題に関するドキュメントへのリンク。</span><span class="sxs-lookup"><span data-stu-id="b5e57-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
