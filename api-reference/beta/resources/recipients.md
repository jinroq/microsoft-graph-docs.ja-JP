---
title: 受信者のリソースの種類
description: 以下は、リソースの JSON 表記です
ms.openlocfilehash: aa620fa920b4f91b2b2214f02c2e75d7a8cbcc4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073202"
---
# <a name="recipients-resource-type"></a><span data-ttu-id="28a88-103">受信者のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="28a88-103">recipients resource type</span></span>

> <span data-ttu-id="28a88-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28a88-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28a88-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28a88-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="28a88-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="28a88-106">JSON representation</span></span>

<span data-ttu-id="28a88-107">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="28a88-107">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="28a88-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28a88-108">Properties</span></span>
| <span data-ttu-id="28a88-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28a88-109">Property</span></span>     | <span data-ttu-id="28a88-110">型</span><span class="sxs-lookup"><span data-stu-id="28a88-110">Type</span></span>   |<span data-ttu-id="28a88-111">説明</span><span class="sxs-lookup"><span data-stu-id="28a88-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28a88-112">alias</span><span class="sxs-lookup"><span data-stu-id="28a88-112">alias</span></span>|<span data-ttu-id="28a88-113">String</span><span class="sxs-lookup"><span data-stu-id="28a88-113">String</span></span>||
|<span data-ttu-id="28a88-114">email</span><span class="sxs-lookup"><span data-stu-id="28a88-114">email</span></span>|<span data-ttu-id="28a88-115">String</span><span class="sxs-lookup"><span data-stu-id="28a88-115">String</span></span>||
|<span data-ttu-id="28a88-116">objectId</span><span class="sxs-lookup"><span data-stu-id="28a88-116">objectId</span></span>|<span data-ttu-id="28a88-117">String</span><span class="sxs-lookup"><span data-stu-id="28a88-117">String</span></span>||
|<span data-ttu-id="28a88-118">permissionIdentityType</span><span class="sxs-lookup"><span data-stu-id="28a88-118">permissionIdentityType</span></span>|<span data-ttu-id="28a88-119">String</span><span class="sxs-lookup"><span data-stu-id="28a88-119">String</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipients resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->