---
title: synchronizationError リソースの種類
description: 同期処理中に発生したエラーを表します。
localization_priority: Normal
ms.openlocfilehash: cc6b58444ac56303bfd2e41f1fcae17658f6aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847244"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="386d0-103">synchronizationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="386d0-103">synchronizationError resource type</span></span>

> <span data-ttu-id="386d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="386d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="386d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="386d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="386d0-106">同期処理中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="386d0-106">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="386d0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="386d0-107">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="386d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="386d0-108">Property</span></span>     | <span data-ttu-id="386d0-109">種類</span><span class="sxs-lookup"><span data-stu-id="386d0-109">Type</span></span>   |<span data-ttu-id="386d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="386d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="386d0-111">code</span><span class="sxs-lookup"><span data-stu-id="386d0-111">code</span></span>|<span data-ttu-id="386d0-112">String</span><span class="sxs-lookup"><span data-stu-id="386d0-112">String</span></span>||
|<span data-ttu-id="386d0-113">message</span><span class="sxs-lookup"><span data-stu-id="386d0-113">message</span></span>|<span data-ttu-id="386d0-114">String</span><span class="sxs-lookup"><span data-stu-id="386d0-114">String</span></span>||
|<span data-ttu-id="386d0-115">tenantActionable</span><span class="sxs-lookup"><span data-stu-id="386d0-115">tenantActionable</span></span>|<span data-ttu-id="386d0-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="386d0-116">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="386d0-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="386d0-117">JSON representation</span></span>

<span data-ttu-id="386d0-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="386d0-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
