---
title: outlookItem リソースの種類
description: 以下は、リソースの JSON 表記です
ms.openlocfilehash: 6de0b5f9f79f8c3f813cbd876fa22f6b43f71a53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073082"
---
# <a name="outlookitem-resource-type"></a><span data-ttu-id="09889-103">outlookItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09889-103">outlookItem resource type</span></span>

> <span data-ttu-id="09889-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09889-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09889-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09889-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09889-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09889-106">JSON representation</span></span>

<span data-ttu-id="09889-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="09889-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="09889-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09889-108">Properties</span></span>
| <span data-ttu-id="09889-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09889-109">Property</span></span>     | <span data-ttu-id="09889-110">型</span><span class="sxs-lookup"><span data-stu-id="09889-110">Type</span></span>   |<span data-ttu-id="09889-111">説明</span><span class="sxs-lookup"><span data-stu-id="09889-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09889-112">categories</span><span class="sxs-lookup"><span data-stu-id="09889-112">categories</span></span>|<span data-ttu-id="09889-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09889-113">String collection</span></span>||
|<span data-ttu-id="09889-114">changeKey</span><span class="sxs-lookup"><span data-stu-id="09889-114">changeKey</span></span>|<span data-ttu-id="09889-115">String</span><span class="sxs-lookup"><span data-stu-id="09889-115">String</span></span>||
|<span data-ttu-id="09889-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09889-116">createdDateTime</span></span>|<span data-ttu-id="09889-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09889-117">DateTimeOffset</span></span>|<span data-ttu-id="09889-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="09889-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="09889-120">id</span><span class="sxs-lookup"><span data-stu-id="09889-120">id</span></span>|<span data-ttu-id="09889-121">String</span><span class="sxs-lookup"><span data-stu-id="09889-121">String</span></span>| <span data-ttu-id="09889-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="09889-122">Read-only.</span></span>|
|<span data-ttu-id="09889-123">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09889-123">lastModifiedDateTime</span></span>|<span data-ttu-id="09889-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09889-124">DateTimeOffset</span></span>|<span data-ttu-id="09889-p103">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="09889-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="relationships"></a><span data-ttu-id="09889-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09889-127">Relationships</span></span>
<span data-ttu-id="09889-128">なし</span><span class="sxs-lookup"><span data-stu-id="09889-128">None</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->