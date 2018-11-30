---
title: 電話リソースの種類
description: 電話番号を表します。
ms.openlocfilehash: d47f2c36f9913eb75868077bdd5bb2d599055c59
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066378"
---
# <a name="phone-resource-type"></a><span data-ttu-id="694f7-103">電話リソースの種類</span><span class="sxs-lookup"><span data-stu-id="694f7-103">phone resource type</span></span>

> <span data-ttu-id="694f7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="694f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="694f7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="694f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="694f7-106">電話番号を表します。</span><span class="sxs-lookup"><span data-stu-id="694f7-106">Represents a phone number.</span></span>


## <a name="properties"></a><span data-ttu-id="694f7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="694f7-107">Properties</span></span>
| <span data-ttu-id="694f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="694f7-108">Property</span></span>     | <span data-ttu-id="694f7-109">型</span><span class="sxs-lookup"><span data-stu-id="694f7-109">Type</span></span>   |<span data-ttu-id="694f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="694f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="694f7-111">数値</span><span class="sxs-lookup"><span data-stu-id="694f7-111">number</span></span>|<span data-ttu-id="694f7-112">文字列</span><span class="sxs-lookup"><span data-stu-id="694f7-112">string</span></span>|<span data-ttu-id="694f7-113">電話番号。</span><span class="sxs-lookup"><span data-stu-id="694f7-113">The phone number.</span></span>|
|<span data-ttu-id="694f7-114">種類</span><span class="sxs-lookup"><span data-stu-id="694f7-114">type</span></span>|<span data-ttu-id="694f7-115">String</span><span class="sxs-lookup"><span data-stu-id="694f7-115">String</span></span>|<span data-ttu-id="694f7-p102">電話番号の種類。可能な値は、`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio` です。</span><span class="sxs-lookup"><span data-stu-id="694f7-p102">The type of phone number. Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="694f7-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="694f7-118">JSON representation</span></span>

<span data-ttu-id="694f7-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="694f7-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.phone"
}-->

```json
{
  "number": "string",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "phone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->