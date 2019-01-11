---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ColumnLink
localization_priority: Normal
ms.openlocfilehash: 226666875b9364f33954e7f932227562a9734267
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888572"
---
# <a name="columnlink-resource-type"></a><span data-ttu-id="91161-102">ColumnLink リソースの種類</span><span class="sxs-lookup"><span data-stu-id="91161-102">ColumnLink resource type</span></span>

> <span data-ttu-id="91161-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91161-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91161-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91161-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="91161-105">[contentType][] の **columnLink** は **columnDefinition** サイトをそのコンテンツ タイプに接続します。</span><span class="sxs-lookup"><span data-stu-id="91161-105">A **columnLink** on a [contentType][] attaches a site **columnDefinition** to that content type.</span></span>

[contentType]: contenttype.md

## <a name="json-representation"></a><span data-ttu-id="91161-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91161-107">JSON representation</span></span>

<span data-ttu-id="91161-108">以下は、**columnLink** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91161-108">Here is a JSON representation of a **columnLink** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnLink" } -->

```json
{
  "id": "string",
  "name": "string"
}
```

## <a name="properties"></a><span data-ttu-id="91161-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91161-109">Properties</span></span>

| <span data-ttu-id="91161-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="91161-110">Property name</span></span> | <span data-ttu-id="91161-111">Type</span><span class="sxs-lookup"><span data-stu-id="91161-111">Type</span></span>   | <span data-ttu-id="91161-112">説明</span><span class="sxs-lookup"><span data-stu-id="91161-112">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="91161-113">**id**</span><span class="sxs-lookup"><span data-stu-id="91161-113">**id**</span></span>        | <span data-ttu-id="91161-114">string</span><span class="sxs-lookup"><span data-stu-id="91161-114">string</span></span> | <span data-ttu-id="91161-115">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="91161-115">The unique identifier for the column.</span></span>
| <span data-ttu-id="91161-116">**name**</span><span class="sxs-lookup"><span data-stu-id="91161-116">**name**</span></span>      | <span data-ttu-id="91161-117">文字列</span><span class="sxs-lookup"><span data-stu-id="91161-117">string</span></span> | <span data-ttu-id="91161-118">このコンテンツ タイプの列の名前。</span><span class="sxs-lookup"><span data-stu-id="91161-118">The name of the column  in this content type.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnLink"
} -->
