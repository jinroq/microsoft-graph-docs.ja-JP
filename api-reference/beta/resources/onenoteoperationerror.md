---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作のエラー。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: ecd1c42ceb278c483601344dd28c72f7436b9537
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009350"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="739cf-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="739cf-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="739cf-104">失敗した OneNote 操作のエラー。</span><span class="sxs-lookup"><span data-stu-id="739cf-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="739cf-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="739cf-105">JSON representation</span></span>

<span data-ttu-id="739cf-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="739cf-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="739cf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="739cf-107">Properties</span></span>
| <span data-ttu-id="739cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="739cf-108">Property</span></span>     | <span data-ttu-id="739cf-109">型</span><span class="sxs-lookup"><span data-stu-id="739cf-109">Type</span></span>   |<span data-ttu-id="739cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="739cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="739cf-111">code</span><span class="sxs-lookup"><span data-stu-id="739cf-111">code</span></span>|<span data-ttu-id="739cf-112">string</span><span class="sxs-lookup"><span data-stu-id="739cf-112">string</span></span>|<span data-ttu-id="739cf-113">エラーコード。</span><span class="sxs-lookup"><span data-stu-id="739cf-113">The error code.</span></span>|
|<span data-ttu-id="739cf-114">message</span><span class="sxs-lookup"><span data-stu-id="739cf-114">message</span></span>|<span data-ttu-id="739cf-115">string</span><span class="sxs-lookup"><span data-stu-id="739cf-115">string</span></span>|<span data-ttu-id="739cf-116">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="739cf-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
