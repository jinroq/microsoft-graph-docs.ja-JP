---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
ms.openlocfilehash: 0dab8b405c99f2931d2cc02cc915df5f805322d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073069"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="a01aa-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a01aa-103">onenoteOperationError resource type</span></span>

> <span data-ttu-id="a01aa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a01aa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a01aa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a01aa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a01aa-106">失敗した OneNote 操作によるエラー。</span><span class="sxs-lookup"><span data-stu-id="a01aa-106">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a01aa-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a01aa-107">JSON representation</span></span>

<span data-ttu-id="a01aa-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a01aa-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a01aa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a01aa-109">Properties</span></span>
| <span data-ttu-id="a01aa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a01aa-110">Property</span></span>     | <span data-ttu-id="a01aa-111">型</span><span class="sxs-lookup"><span data-stu-id="a01aa-111">Type</span></span>   |<span data-ttu-id="a01aa-112">説明</span><span class="sxs-lookup"><span data-stu-id="a01aa-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a01aa-113">code</span><span class="sxs-lookup"><span data-stu-id="a01aa-113">code</span></span>|<span data-ttu-id="a01aa-114">文字列</span><span class="sxs-lookup"><span data-stu-id="a01aa-114">string</span></span>|<span data-ttu-id="a01aa-115">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="a01aa-115">The error code.</span></span>|
|<span data-ttu-id="a01aa-116">message</span><span class="sxs-lookup"><span data-stu-id="a01aa-116">message</span></span>|<span data-ttu-id="a01aa-117">文字列</span><span class="sxs-lookup"><span data-stu-id="a01aa-117">string</span></span>|<span data-ttu-id="a01aa-118">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="a01aa-118">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
