---
title: operationError リソースの種類
description: TeamsAsyncOperation で発生したエラーをについて説明します。
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023189"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="644fd-103">operationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="644fd-103">operationError resource type</span></span>



<span data-ttu-id="644fd-104">[TeamsAsyncOperation](teamsasyncoperation.md)で発生したエラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="644fd-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="644fd-105">operationError プロパティ</span><span class="sxs-lookup"><span data-stu-id="644fd-105">operationError Properties</span></span>
| <span data-ttu-id="644fd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="644fd-106">Property</span></span>     | <span data-ttu-id="644fd-107">型</span><span class="sxs-lookup"><span data-stu-id="644fd-107">Type</span></span>   |<span data-ttu-id="644fd-108">説明</span><span class="sxs-lookup"><span data-stu-id="644fd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="644fd-109">code</span><span class="sxs-lookup"><span data-stu-id="644fd-109">code</span></span>|<span data-ttu-id="644fd-110">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="644fd-110">string (readonly)</span></span>|<span data-ttu-id="644fd-111">操作のエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="644fd-111">Operation error code.</span></span>|
|<span data-ttu-id="644fd-112">message</span><span class="sxs-lookup"><span data-stu-id="644fd-112">message</span></span>|<span data-ttu-id="644fd-113">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="644fd-113">string (readonly)</span></span>|<span data-ttu-id="644fd-114">エラー メッセージを操作します。</span><span class="sxs-lookup"><span data-stu-id="644fd-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="644fd-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="644fd-115">JSON representation</span></span>

<span data-ttu-id="644fd-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="644fd-116">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
