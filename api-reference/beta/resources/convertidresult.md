---
title: convertIdResult リソースの種類
description: TranslateExchangeIds 関数によって実行される ID 形式変換の結果です。
ms.openlocfilehash: 3a17399ffe44c43c78f7b50933b2e847a3e64f32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067806"
---
# <a name="convertidresult-resource-type"></a><span data-ttu-id="9f02c-103">convertIdResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f02c-103">convertIdResult resource type</span></span>

> <span data-ttu-id="9f02c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9f02c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9f02c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f02c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9f02c-106">[TranslateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果です。</span><span class="sxs-lookup"><span data-stu-id="9f02c-106">The result of an ID format conversion performed by the [translateExchangeIds](../api/user-translateexchangeids.md) function.</span></span>

## <a name="properties"></a><span data-ttu-id="9f02c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f02c-107">Properties</span></span>

| <span data-ttu-id="9f02c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f02c-108">Property</span></span> | <span data-ttu-id="9f02c-109">型</span><span class="sxs-lookup"><span data-stu-id="9f02c-109">Type</span></span> | <span data-ttu-id="9f02c-110">説明</span><span class="sxs-lookup"><span data-stu-id="9f02c-110">Description</span></span> |
|:---------|:-----|:------------|
| <span data-ttu-id="9f02c-111">sourceId</span><span class="sxs-lookup"><span data-stu-id="9f02c-111">sourceId</span></span> | <span data-ttu-id="9f02c-112">String</span><span class="sxs-lookup"><span data-stu-id="9f02c-112">String</span></span> | <span data-ttu-id="9f02c-113">変換された識別子です。</span><span class="sxs-lookup"><span data-stu-id="9f02c-113">The identifier that was converted.</span></span> <span data-ttu-id="9f02c-114">この値は、元、変換されていない識別子です。</span><span class="sxs-lookup"><span data-stu-id="9f02c-114">This value is the original, un-converted identifier.</span></span> |
| <span data-ttu-id="9f02c-115">targetId</span><span class="sxs-lookup"><span data-stu-id="9f02c-115">targetId</span></span> | <span data-ttu-id="9f02c-116">String</span><span class="sxs-lookup"><span data-stu-id="9f02c-116">String</span></span> | <span data-ttu-id="9f02c-117">変換後の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9f02c-117">The converted identifier.</span></span> <span data-ttu-id="9f02c-118">この値は、変換が失敗した場合ではありません。</span><span class="sxs-lookup"><span data-stu-id="9f02c-118">This value is not present if the conversion failed.</span></span> |
| <span data-ttu-id="9f02c-119">errorDetails</span><span class="sxs-lookup"><span data-stu-id="9f02c-119">errorDetails</span></span> | [<span data-ttu-id="9f02c-120">genericError</span><span class="sxs-lookup"><span data-stu-id="9f02c-120">genericError</span></span>](genericerror.md) | <span data-ttu-id="9f02c-121">変換エラーの原因を示すエラー オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9f02c-121">An error object indicating the reason for the conversion failure.</span></span> <span data-ttu-id="9f02c-122">この値は、変換が成功した場合ではありません。</span><span class="sxs-lookup"><span data-stu-id="9f02c-122">This value is not present if the conversion succeeded.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9f02c-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f02c-123">JSON representation</span></span>

<span data-ttu-id="9f02c-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9f02c-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```