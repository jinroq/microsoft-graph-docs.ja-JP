---
title: domainState リソースの種類
description: ドメイン上でスケジュールされている非同期操作の状態を表します。
author: lleonard-msft
ms.openlocfilehash: 683390998254cbf3f7146d1fe89a0a2f109be320
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355889"
---
# <a name="domainstate-resource-type"></a><span data-ttu-id="44893-103">domainState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="44893-103">domainState resource type</span></span>

> <span data-ttu-id="44893-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44893-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="44893-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44893-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="44893-106">ドメイン上でスケジュールされている非同期操作の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="44893-106">Represents the status of asynchronous operations scheduled on a domain.</span></span>

## <a name="properties"></a><span data-ttu-id="44893-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44893-107">Properties</span></span>

| <span data-ttu-id="44893-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44893-108">Property</span></span>   | <span data-ttu-id="44893-109">種類</span><span class="sxs-lookup"><span data-stu-id="44893-109">Type</span></span> | <span data-ttu-id="44893-110">説明</span><span class="sxs-lookup"><span data-stu-id="44893-110">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="44893-111">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="44893-111">lastActionDateTime</span></span> | <span data-ttu-id="44893-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44893-112">DateTimeOffset</span></span> | <span data-ttu-id="44893-p102">最後のアクティビティが発生したときのタイムスタンプ。値は、操作のスケジュール時、非同期タスクの開始時、操作の完了時に更新されます。</span><span class="sxs-lookup"><span data-stu-id="44893-p102">Timestamp for when the last activity occurred. The value is updated when an operation is scheduled, the asynchronous task starts, and when the operation completes.</span></span> |
| <span data-ttu-id="44893-115">操作​​</span><span class="sxs-lookup"><span data-stu-id="44893-115">operation</span></span> | <span data-ttu-id="44893-116">String</span><span class="sxs-lookup"><span data-stu-id="44893-116">String</span></span> | <span data-ttu-id="44893-p103">非同期操作の種類。値は、*ForceDelete* または *Verification* のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="44893-p103">Type of asynchronous operation. The values can be *ForceDelete* or *Verification*</span></span> |
| <span data-ttu-id="44893-119">status</span><span class="sxs-lookup"><span data-stu-id="44893-119">status</span></span> | <span data-ttu-id="44893-120">String</span><span class="sxs-lookup"><span data-stu-id="44893-120">String</span></span> | <span data-ttu-id="44893-121">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="44893-121">Current status of the operation.</span></span> <br> <span data-ttu-id="44893-122">*Scheduled* - 操作はスケジュールされていますが、開始されていません。</span><span class="sxs-lookup"><span data-stu-id="44893-122">*Scheduled* - Operation has been scheduled but has not started.</span></span> <br> <span data-ttu-id="44893-123">*InProgress* - タスクが開始され、実行中です。</span><span class="sxs-lookup"><span data-stu-id="44893-123">*InProgress* - Task has started and is in progress.</span></span> <br> <span data-ttu-id="44893-124">*Failed* - 操作が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="44893-124">*Failed* - Operation has failed.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="44893-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="44893-125">JSON representation</span></span>
<span data-ttu-id="44893-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="44893-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainState"
}-->

```json
{
  "lastActionDateTime": "String (timestamp)",
  "operation": "String",
  "status": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->