---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 998b62b639bb155e320d8293452052d8eebe41ca
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952518"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="bf559-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bf559-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="bf559-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf559-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf559-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf559-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf559-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf559-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bf559-107">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="bf559-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="bf559-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf559-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bf559-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf559-109">Properties</span></span>
|<span data-ttu-id="bf559-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf559-110">Property</span></span>|<span data-ttu-id="bf559-111">種類</span><span class="sxs-lookup"><span data-stu-id="bf559-111">Type</span></span>|<span data-ttu-id="bf559-112">説明</span><span class="sxs-lookup"><span data-stu-id="bf559-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf559-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bf559-113">displayName</span></span>|<span data-ttu-id="bf559-114">文字列</span><span class="sxs-lookup"><span data-stu-id="bf559-114">String</span></span>|<span data-ttu-id="bf559-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="bf559-115">Display Name.</span></span> <span data-ttu-id="bf559-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf559-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bf559-117">説明</span><span class="sxs-lookup"><span data-stu-id="bf559-117">description</span></span>|<span data-ttu-id="bf559-118">String</span><span class="sxs-lookup"><span data-stu-id="bf559-118">String</span></span>|<span data-ttu-id="bf559-119">説明。</span><span class="sxs-lookup"><span data-stu-id="bf559-119">Description.</span></span> <span data-ttu-id="bf559-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf559-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bf559-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="bf559-121">omaUri</span></span>|<span data-ttu-id="bf559-122">文字列</span><span class="sxs-lookup"><span data-stu-id="bf559-122">String</span></span>|<span data-ttu-id="bf559-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="bf559-123">OMA.</span></span> <span data-ttu-id="bf559-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bf559-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bf559-125">値</span><span class="sxs-lookup"><span data-stu-id="bf559-125">value</span></span>|<span data-ttu-id="bf559-126">Int32</span><span class="sxs-lookup"><span data-stu-id="bf559-126">Int32</span></span>|<span data-ttu-id="bf559-127">値。</span><span class="sxs-lookup"><span data-stu-id="bf559-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf559-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bf559-128">Relationships</span></span>
<span data-ttu-id="bf559-129">なし</span><span class="sxs-lookup"><span data-stu-id="bf559-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bf559-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf559-130">JSON Representation</span></span>
<span data-ttu-id="bf559-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf559-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```





