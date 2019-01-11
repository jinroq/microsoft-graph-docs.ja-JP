---
title: 診断のリソースの種類
description: エラーまたは OneNote の操作のための警告について説明します。
localization_priority: Normal
ms.openlocfilehash: 28cdd1c07bab0494a69cfb7ce6a5284238e1ff19
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845991"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="922ec-103">診断のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="922ec-103">diagnostic resource type</span></span>

> <span data-ttu-id="922ec-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="922ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="922ec-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="922ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="922ec-106">エラーまたは OneNote の操作のための警告について説明します。</span><span class="sxs-lookup"><span data-stu-id="922ec-106">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="922ec-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="922ec-107">JSON representation</span></span>

<span data-ttu-id="922ec-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="922ec-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="922ec-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="922ec-109">Properties</span></span>
| <span data-ttu-id="922ec-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="922ec-110">Property</span></span>     | <span data-ttu-id="922ec-111">種類</span><span class="sxs-lookup"><span data-stu-id="922ec-111">Type</span></span>   |<span data-ttu-id="922ec-112">説明</span><span class="sxs-lookup"><span data-stu-id="922ec-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="922ec-113">message</span><span class="sxs-lookup"><span data-stu-id="922ec-113">message</span></span>|<span data-ttu-id="922ec-114">String</span><span class="sxs-lookup"><span data-stu-id="922ec-114">String</span></span>|<span data-ttu-id="922ec-115">エラーまたは警告の原因となった状態を示すメッセージです。</span><span class="sxs-lookup"><span data-stu-id="922ec-115">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="922ec-116">url</span><span class="sxs-lookup"><span data-stu-id="922ec-116">url</span></span>|<span data-ttu-id="922ec-117">String</span><span class="sxs-lookup"><span data-stu-id="922ec-117">String</span></span>|<span data-ttu-id="922ec-118">この問題は、ドキュメントをリンクします。</span><span class="sxs-lookup"><span data-stu-id="922ec-118">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
