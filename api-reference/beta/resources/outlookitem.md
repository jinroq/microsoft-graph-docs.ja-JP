---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: b88a450465798386ad57e82ff76896417301a606
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817634"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="a9b8e-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a9b8e-103">outlookItem resource type</span></span>

> <span data-ttu-id="a9b8e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9b8e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9b8e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9b8e-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a9b8e-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a9b8e-106">JSON representation</span></span>

<span data-ttu-id="a9b8e-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a9b8e-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="a9b8e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9b8e-108">Properties</span></span>
| <span data-ttu-id="a9b8e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9b8e-109">Property</span></span>     | <span data-ttu-id="a9b8e-110">種類</span><span class="sxs-lookup"><span data-stu-id="a9b8e-110">Type</span></span>   |<span data-ttu-id="a9b8e-111">説明</span><span class="sxs-lookup"><span data-stu-id="a9b8e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9b8e-112">categories</span><span class="sxs-lookup"><span data-stu-id="a9b8e-112">categories</span></span>|<span data-ttu-id="a9b8e-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a9b8e-113">String collection</span></span>||
|<span data-ttu-id="a9b8e-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="a9b8e-114">changeKey</span></span>|<span data-ttu-id="a9b8e-115">String</span><span class="sxs-lookup"><span data-stu-id="a9b8e-115">String</span></span>||
|<span data-ttu-id="a9b8e-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a9b8e-116">createdDateTime</span></span>|<span data-ttu-id="a9b8e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9b8e-117">DateTimeOffset</span></span>|<span data-ttu-id="a9b8e-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a9b8e-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a9b8e-120">id</span><span class="sxs-lookup"><span data-stu-id="a9b8e-120">id</span></span>|<span data-ttu-id="a9b8e-121">String</span><span class="sxs-lookup"><span data-stu-id="a9b8e-121">String</span></span>| <span data-ttu-id="a9b8e-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9b8e-122">Read-only.</span></span>|
|<span data-ttu-id="a9b8e-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9b8e-123">lastModifiedDateTime</span></span>|<span data-ttu-id="a9b8e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9b8e-124">DateTimeOffset</span></span>|<span data-ttu-id="a9b8e-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a9b8e-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9b8e-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a9b8e-127">Relationships</span></span>
<span data-ttu-id="a9b8e-128">なし</span><span class="sxs-lookup"><span data-stu-id="a9b8e-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
