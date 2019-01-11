---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: cfe859bea40f15311a631e8b1d2b3c3a3c179d0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891533"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="e89a0-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e89a0-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="e89a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e89a0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e89a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e89a0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e89a0-106">失敗した OneNote 操作によるエラー。</span><span class="sxs-lookup"><span data-stu-id="e89a0-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e89a0-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e89a0-107">JSON representation</span></span>

<span data-ttu-id="e89a0-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e89a0-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e89a0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e89a0-109">Properties</span></span>
| <span data-ttu-id="e89a0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e89a0-110">Property</span></span>     | <span data-ttu-id="e89a0-111">種類</span><span class="sxs-lookup"><span data-stu-id="e89a0-111">Type</span></span>   |<span data-ttu-id="e89a0-112">説明</span><span class="sxs-lookup"><span data-stu-id="e89a0-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e89a0-113">code</span><span class="sxs-lookup"><span data-stu-id="e89a0-113">code</span></span>|<span data-ttu-id="e89a0-114">文字列</span><span class="sxs-lookup"><span data-stu-id="e89a0-114">string</span></span>|<span data-ttu-id="e89a0-115">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="e89a0-115">The error code.</span></span>|
|<span data-ttu-id="e89a0-116">message</span><span class="sxs-lookup"><span data-stu-id="e89a0-116">message</span></span>|<span data-ttu-id="e89a0-117">文字列</span><span class="sxs-lookup"><span data-stu-id="e89a0-117">string</span></span>|<span data-ttu-id="e89a0-118">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="e89a0-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
