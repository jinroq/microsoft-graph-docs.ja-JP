---
title: mailTipsError リソースの種類
description: 操作中に発生するエラーです。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b9efff5538d7eb6be0fe468f70a4ff59ddf9d14a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916202"
---
# <a name="mailtipserror-resource-type"></a><span data-ttu-id="27049-103">mailTipsError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27049-103">mailTipsError resource type</span></span>

> <span data-ttu-id="27049-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27049-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27049-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27049-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27049-106">操作中に発生するエラーです。</span><span class="sxs-lookup"><span data-stu-id="27049-106">An error that occurs during an action.</span></span>

## <a name="properties"></a><span data-ttu-id="27049-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27049-107">Properties</span></span>
| <span data-ttu-id="27049-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27049-108">Property</span></span>     | <span data-ttu-id="27049-109">種類</span><span class="sxs-lookup"><span data-stu-id="27049-109">Type</span></span>   |<span data-ttu-id="27049-110">説明</span><span class="sxs-lookup"><span data-stu-id="27049-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="27049-111">message</span><span class="sxs-lookup"><span data-stu-id="27049-111">message</span></span> | <span data-ttu-id="27049-112">String</span><span class="sxs-lookup"><span data-stu-id="27049-112">String</span></span> | <span data-ttu-id="27049-113">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="27049-113">The error message.</span></span> |
| <span data-ttu-id="27049-114">code</span><span class="sxs-lookup"><span data-stu-id="27049-114">code</span></span> | <span data-ttu-id="27049-115">String</span><span class="sxs-lookup"><span data-stu-id="27049-115">String</span></span> | <span data-ttu-id="27049-116">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="27049-116">The error code.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27049-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27049-117">JSON representation</span></span>

<span data-ttu-id="27049-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="27049-118">Here is a JSON representation of the resource.</span></span>

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
