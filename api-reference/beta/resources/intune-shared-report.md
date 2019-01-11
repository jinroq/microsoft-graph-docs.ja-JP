---
title: レポート リソースの種類
description: コンテキストに適切なコンテンツを返すなど。
localization_priority: Normal
ms.openlocfilehash: b44d03c12b788b10ca332c868083bc28decc4947
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875727"
---
# <a name="report-resource-type"></a><span data-ttu-id="43918-103">レポート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43918-103">report resource type</span></span>

> <span data-ttu-id="43918-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="43918-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43918-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43918-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="43918-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="43918-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43918-107">コンテキストに適切なコンテンツを返すなど。</span><span class="sxs-lookup"><span data-stu-id="43918-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="43918-108">デバイス構成のプロファイルの履歴のレポートです。</span><span class="sxs-lookup"><span data-stu-id="43918-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="43918-109">障害レポートを登録します。</span><span class="sxs-lookup"><span data-stu-id="43918-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="43918-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43918-110">Properties</span></span>
|<span data-ttu-id="43918-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43918-111">Property</span></span>|<span data-ttu-id="43918-112">種類</span><span class="sxs-lookup"><span data-stu-id="43918-112">Type</span></span>|<span data-ttu-id="43918-113">説明</span><span class="sxs-lookup"><span data-stu-id="43918-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43918-114">content</span><span class="sxs-lookup"><span data-stu-id="43918-114">content</span></span>|<span data-ttu-id="43918-115">Stream</span><span class="sxs-lookup"><span data-stu-id="43918-115">Stream</span></span>|<span data-ttu-id="43918-116">レポート コンテンツです。詳細は、レポートの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="43918-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43918-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="43918-117">Relationships</span></span>
<span data-ttu-id="43918-118">なし</span><span class="sxs-lookup"><span data-stu-id="43918-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43918-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43918-119">JSON Representation</span></span>
<span data-ttu-id="43918-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43918-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



