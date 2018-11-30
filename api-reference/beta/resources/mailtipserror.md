---
title: mailTipsError リソースの種類
description: 操作中に発生するエラーです。
ms.openlocfilehash: 94ab795d5cb12c2ff8490806326968d363e1a761
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073019"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="16d24-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16d24-103">mailTipsError resource type</span></span>

> <span data-ttu-id="16d24-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16d24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16d24-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16d24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16d24-106">操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="16d24-106">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="16d24-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d24-107">Properties</span></span>
| <span data-ttu-id="16d24-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16d24-108">Property</span></span>     | <span data-ttu-id="16d24-109">型</span><span class="sxs-lookup"><span data-stu-id="16d24-109">Type</span></span>   |<span data-ttu-id="16d24-110">説明</span><span class="sxs-lookup"><span data-stu-id="16d24-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="16d24-111">message</span><span class="sxs-lookup"><span data-stu-id="16d24-111">message</span></span> | <span data-ttu-id="16d24-112">String</span><span class="sxs-lookup"><span data-stu-id="16d24-112">String</span></span> | <span data-ttu-id="16d24-113">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="16d24-113">The error message.</span></span> |
| <span data-ttu-id="16d24-114">code</span><span class="sxs-lookup"><span data-stu-id="16d24-114">code</span></span> | <span data-ttu-id="16d24-115">String</span><span class="sxs-lookup"><span data-stu-id="16d24-115">String</span></span> | <span data-ttu-id="16d24-116">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="16d24-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="16d24-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16d24-117">JSON representation</span></span>

<span data-ttu-id="16d24-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="16d24-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mailTipsError"
}-->

```json
{
  "message": "string",
  "code": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailTipsError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->