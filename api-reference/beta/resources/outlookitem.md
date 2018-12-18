---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
author: angelgolfer-ms
ms.openlocfilehash: 4d375606a5104d48955561df3b904922a5daf042
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315023"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="56bd6-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56bd6-103">outlookItem resource type</span></span>

> <span data-ttu-id="56bd6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56bd6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56bd6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56bd6-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="56bd6-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56bd6-106">JSON representation</span></span>

<span data-ttu-id="56bd6-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="56bd6-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookitem"
}-->

```json
{
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}

```
## <a name="properties"></a><span data-ttu-id="56bd6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56bd6-108">Properties</span></span>
| <span data-ttu-id="56bd6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56bd6-109">Property</span></span>     | <span data-ttu-id="56bd6-110">種類</span><span class="sxs-lookup"><span data-stu-id="56bd6-110">Type</span></span>   |<span data-ttu-id="56bd6-111">説明</span><span class="sxs-lookup"><span data-stu-id="56bd6-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56bd6-112">categories</span><span class="sxs-lookup"><span data-stu-id="56bd6-112">categories</span></span>|<span data-ttu-id="56bd6-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="56bd6-113">String collection</span></span>||
|<span data-ttu-id="56bd6-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="56bd6-114">changeKey</span></span>|<span data-ttu-id="56bd6-115">String</span><span class="sxs-lookup"><span data-stu-id="56bd6-115">String</span></span>||
|<span data-ttu-id="56bd6-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56bd6-116">createdDateTime</span></span>|<span data-ttu-id="56bd6-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bd6-117">DateTimeOffset</span></span>|<span data-ttu-id="56bd6-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="56bd6-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="56bd6-120">id</span><span class="sxs-lookup"><span data-stu-id="56bd6-120">id</span></span>|<span data-ttu-id="56bd6-121">String</span><span class="sxs-lookup"><span data-stu-id="56bd6-121">String</span></span>| <span data-ttu-id="56bd6-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="56bd6-122">Read-only.</span></span>|
|<span data-ttu-id="56bd6-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56bd6-123">lastModifiedDateTime</span></span>|<span data-ttu-id="56bd6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bd6-124">DateTimeOffset</span></span>|<span data-ttu-id="56bd6-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="56bd6-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="56bd6-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="56bd6-127">Relationships</span></span>
<span data-ttu-id="56bd6-128">なし</span><span class="sxs-lookup"><span data-stu-id="56bd6-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->