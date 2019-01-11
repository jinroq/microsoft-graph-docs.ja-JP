---
title: 受信者のリソースの種類
description: 以下は、リソースの JSON 表記です
localization_priority: Normal
ms.openlocfilehash: c0afde5b7bd427389b5b81be055781dfaff194e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829585"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="12e13-103">受信者のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="12e13-103">recipients resource type</span></span>

> <span data-ttu-id="12e13-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="12e13-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12e13-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12e13-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12e13-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12e13-106">JSON representation</span></span>

<span data-ttu-id="12e13-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="12e13-107">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipients"
}-->

```json
{
  "alias": "string",
  "email": "string",
  "objectId": "string",
  "permissionIdentityType": "string"
}

```
## <a name="properties"></a><span data-ttu-id="12e13-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12e13-108">Properties</span></span>
| <span data-ttu-id="12e13-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12e13-109">Property</span></span>     | <span data-ttu-id="12e13-110">種類</span><span class="sxs-lookup"><span data-stu-id="12e13-110">Type</span></span>   |<span data-ttu-id="12e13-111">説明</span><span class="sxs-lookup"><span data-stu-id="12e13-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12e13-112">alias</span><span class="sxs-lookup"><span data-stu-id="12e13-112">alias</span></span>|<span data-ttu-id="12e13-113">String</span><span class="sxs-lookup"><span data-stu-id="12e13-113">String</span></span>||
|<span data-ttu-id="12e13-114">email</span><span class="sxs-lookup"><span data-stu-id="12e13-114">email</span></span>|<span data-ttu-id="12e13-115">String</span><span class="sxs-lookup"><span data-stu-id="12e13-115">String</span></span>||
|<span data-ttu-id="12e13-116">objectId</span><span class="sxs-lookup"><span data-stu-id="12e13-116">objectId</span></span>|<span data-ttu-id="12e13-117">String</span><span class="sxs-lookup"><span data-stu-id="12e13-117">String</span></span>||
|<span data-ttu-id="12e13-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="12e13-118">permissionIdentityType</span></span>|<span data-ttu-id="12e13-119">String</span><span class="sxs-lookup"><span data-stu-id="12e13-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
