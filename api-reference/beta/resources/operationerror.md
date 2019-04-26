---
title: operationerror リソースの種類
description: teamsAsyncOperation のエラーについて説明します。
localization_priority: Normal
ms.openlocfilehash: 1f07fe064d7bbd255f2693071c86842a34fdffa0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568914"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="7f581-103">operationerror リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f581-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f581-104">[teamsAsyncOperation](teamsasyncoperation.md)のエラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7f581-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="7f581-105">operationerror プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f581-105">operationError Properties</span></span>
| <span data-ttu-id="7f581-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f581-106">Property</span></span>     | <span data-ttu-id="7f581-107">型</span><span class="sxs-lookup"><span data-stu-id="7f581-107">Type</span></span>   |<span data-ttu-id="7f581-108">説明</span><span class="sxs-lookup"><span data-stu-id="7f581-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f581-109">code</span><span class="sxs-lookup"><span data-stu-id="7f581-109">code</span></span>|<span data-ttu-id="7f581-110">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="7f581-110">string (readonly)</span></span>|<span data-ttu-id="7f581-111">操作エラーコード。</span><span class="sxs-lookup"><span data-stu-id="7f581-111">Operation error code.</span></span>|
|<span data-ttu-id="7f581-112">message</span><span class="sxs-lookup"><span data-stu-id="7f581-112">message</span></span>|<span data-ttu-id="7f581-113">string (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="7f581-113">string (readonly)</span></span>|<span data-ttu-id="7f581-114">操作エラーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="7f581-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f581-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f581-115">JSON representation</span></span>

<span data-ttu-id="7f581-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f581-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
