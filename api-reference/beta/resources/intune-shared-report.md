---
title: レポート リソースの種類
description: Intune は、複数のワークフローをサポートする Microsoft グラフ API のレポートのリソースについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 098c20b2460324c4975533902e1b71fde1af41c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407474"
---
# <a name="report-resource-type"></a><span data-ttu-id="925ce-103">レポート リソースの種類</span><span class="sxs-lookup"><span data-stu-id="925ce-103">report resource type</span></span>

> <span data-ttu-id="925ce-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="925ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="925ce-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="925ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="925ce-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="925ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="925ce-107">コンテキストに適切なコンテンツを返すなど。</span><span class="sxs-lookup"><span data-stu-id="925ce-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="925ce-108">デバイス構成のプロファイルの履歴のレポートです。</span><span class="sxs-lookup"><span data-stu-id="925ce-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="925ce-109">障害レポートを登録します。</span><span class="sxs-lookup"><span data-stu-id="925ce-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="925ce-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="925ce-110">Properties</span></span>
|<span data-ttu-id="925ce-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="925ce-111">Property</span></span>|<span data-ttu-id="925ce-112">型</span><span class="sxs-lookup"><span data-stu-id="925ce-112">Type</span></span>|<span data-ttu-id="925ce-113">説明</span><span class="sxs-lookup"><span data-stu-id="925ce-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="925ce-114">content</span><span class="sxs-lookup"><span data-stu-id="925ce-114">content</span></span>|<span data-ttu-id="925ce-115">Stream</span><span class="sxs-lookup"><span data-stu-id="925ce-115">Stream</span></span>|<span data-ttu-id="925ce-116">レポート コンテンツです。詳細は、レポートの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="925ce-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="925ce-117">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="925ce-117">Relationships</span></span>
<span data-ttu-id="925ce-118">なし</span><span class="sxs-lookup"><span data-stu-id="925ce-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="925ce-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="925ce-119">JSON Representation</span></span>
<span data-ttu-id="925ce-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="925ce-120">Here is a JSON representation of the resource.</span></span>
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



