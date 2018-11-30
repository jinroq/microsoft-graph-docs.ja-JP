---
title: レポート リソースの種類
description: コンテキストに適切なコンテンツを返すなど。
ms.openlocfilehash: b05e5db2b948455f14746cf23a07b3fd788ccad9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071886"
---
# <a name="report-resource-type"></a><span data-ttu-id="474d1-103">レポート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="474d1-103">report resource type</span></span>

> <span data-ttu-id="474d1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="474d1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="474d1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="474d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="474d1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="474d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="474d1-107">コンテキストに適切なコンテンツを返すなど。</span><span class="sxs-lookup"><span data-stu-id="474d1-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="474d1-108">デバイス構成のプロファイルの履歴のレポートです。</span><span class="sxs-lookup"><span data-stu-id="474d1-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="474d1-109">障害レポートを登録します。</span><span class="sxs-lookup"><span data-stu-id="474d1-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="474d1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="474d1-110">Properties</span></span>
|<span data-ttu-id="474d1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="474d1-111">Property</span></span>|<span data-ttu-id="474d1-112">型</span><span class="sxs-lookup"><span data-stu-id="474d1-112">Type</span></span>|<span data-ttu-id="474d1-113">説明</span><span class="sxs-lookup"><span data-stu-id="474d1-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="474d1-114">content</span><span class="sxs-lookup"><span data-stu-id="474d1-114">content</span></span>|<span data-ttu-id="474d1-115">Stream</span><span class="sxs-lookup"><span data-stu-id="474d1-115">Stream</span></span>|<span data-ttu-id="474d1-116">レポート コンテンツです。詳細は、レポートの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="474d1-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="474d1-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="474d1-117">Relationships</span></span>
<span data-ttu-id="474d1-118">なし</span><span class="sxs-lookup"><span data-stu-id="474d1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="474d1-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="474d1-119">JSON Representation</span></span>
<span data-ttu-id="474d1-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="474d1-120">Here is a JSON representation of the resource.</span></span>
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



