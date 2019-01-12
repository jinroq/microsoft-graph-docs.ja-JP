---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4552eef8ec9237c45b1e2b98404977a48e99a896
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942543"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="2324d-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2324d-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="2324d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2324d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2324d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2324d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2324d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2324d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2324d-107">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="2324d-107">OMA Settings DateTime definition.</span></span>

<span data-ttu-id="2324d-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2324d-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2324d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2324d-109">Properties</span></span>
|<span data-ttu-id="2324d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2324d-110">Property</span></span>|<span data-ttu-id="2324d-111">種類</span><span class="sxs-lookup"><span data-stu-id="2324d-111">Type</span></span>|<span data-ttu-id="2324d-112">説明</span><span class="sxs-lookup"><span data-stu-id="2324d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2324d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="2324d-113">displayName</span></span>|<span data-ttu-id="2324d-114">文字列</span><span class="sxs-lookup"><span data-stu-id="2324d-114">String</span></span>|<span data-ttu-id="2324d-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="2324d-115">Display Name.</span></span> <span data-ttu-id="2324d-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2324d-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2324d-117">説明</span><span class="sxs-lookup"><span data-stu-id="2324d-117">description</span></span>|<span data-ttu-id="2324d-118">String</span><span class="sxs-lookup"><span data-stu-id="2324d-118">String</span></span>|<span data-ttu-id="2324d-119">説明。</span><span class="sxs-lookup"><span data-stu-id="2324d-119">Description.</span></span> <span data-ttu-id="2324d-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2324d-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2324d-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="2324d-121">omaUri</span></span>|<span data-ttu-id="2324d-122">文字列</span><span class="sxs-lookup"><span data-stu-id="2324d-122">String</span></span>|<span data-ttu-id="2324d-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="2324d-123">OMA.</span></span> <span data-ttu-id="2324d-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2324d-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2324d-125">値</span><span class="sxs-lookup"><span data-stu-id="2324d-125">value</span></span>|<span data-ttu-id="2324d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2324d-126">DateTimeOffset</span></span>|<span data-ttu-id="2324d-127">値。</span><span class="sxs-lookup"><span data-stu-id="2324d-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2324d-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2324d-128">Relationships</span></span>
<span data-ttu-id="2324d-129">なし</span><span class="sxs-lookup"><span data-stu-id="2324d-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2324d-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2324d-130">JSON Representation</span></span>
<span data-ttu-id="2324d-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2324d-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```





