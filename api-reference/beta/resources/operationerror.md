---
title: operationError リソースの種類
description: TeamsAsyncOperation で発生したエラーをについて説明します。
localization_priority: Normal
ms.openlocfilehash: 423f426df92e99754af0abf4c9c8088eea61d5ea
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890294"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="93ead-103">operationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93ead-103">operationError resource type</span></span>

> <span data-ttu-id="93ead-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="93ead-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="93ead-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="93ead-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="93ead-106">[TeamsAsyncOperation](teamsasyncoperation.md)で発生したエラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="93ead-106">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="93ead-107">operationError プロパティ</span><span class="sxs-lookup"><span data-stu-id="93ead-107">operationError Properties</span></span>
| <span data-ttu-id="93ead-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93ead-108">Property</span></span>     | <span data-ttu-id="93ead-109">種類</span><span class="sxs-lookup"><span data-stu-id="93ead-109">Type</span></span>   |<span data-ttu-id="93ead-110">説明</span><span class="sxs-lookup"><span data-stu-id="93ead-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93ead-111">code</span><span class="sxs-lookup"><span data-stu-id="93ead-111">code</span></span>|<span data-ttu-id="93ead-112">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="93ead-112">string (readonly)</span></span>|<span data-ttu-id="93ead-113">操作のエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="93ead-113">Operation error code.</span></span>|
|<span data-ttu-id="93ead-114">message</span><span class="sxs-lookup"><span data-stu-id="93ead-114">message</span></span>|<span data-ttu-id="93ead-115">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="93ead-115">string (readonly)</span></span>|<span data-ttu-id="93ead-116">エラー メッセージを操作します。</span><span class="sxs-lookup"><span data-stu-id="93ead-116">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93ead-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93ead-117">JSON representation</span></span>

<span data-ttu-id="93ead-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93ead-118">The following is a JSON representation of the resource.</span></span>

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
