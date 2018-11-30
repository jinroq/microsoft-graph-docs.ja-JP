---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
ms.openlocfilehash: fe435146cc0ab8a4c97f12c443e0c30ad0ca78ec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069115"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="6745c-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6745c-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="6745c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6745c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6745c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6745c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6745c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6745c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6745c-107">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="6745c-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="6745c-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6745c-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6745c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6745c-109">Properties</span></span>
|<span data-ttu-id="6745c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6745c-110">Property</span></span>|<span data-ttu-id="6745c-111">型</span><span class="sxs-lookup"><span data-stu-id="6745c-111">Type</span></span>|<span data-ttu-id="6745c-112">説明</span><span class="sxs-lookup"><span data-stu-id="6745c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6745c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6745c-113">displayName</span></span>|<span data-ttu-id="6745c-114">文字列</span><span class="sxs-lookup"><span data-stu-id="6745c-114">String</span></span>|<span data-ttu-id="6745c-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="6745c-115">Display Name.</span></span> <span data-ttu-id="6745c-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6745c-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6745c-117">説明</span><span class="sxs-lookup"><span data-stu-id="6745c-117">description</span></span>|<span data-ttu-id="6745c-118">String</span><span class="sxs-lookup"><span data-stu-id="6745c-118">String</span></span>|<span data-ttu-id="6745c-119">説明。</span><span class="sxs-lookup"><span data-stu-id="6745c-119">Description.</span></span> <span data-ttu-id="6745c-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6745c-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6745c-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="6745c-121">omaUri</span></span>|<span data-ttu-id="6745c-122">文字列</span><span class="sxs-lookup"><span data-stu-id="6745c-122">String</span></span>|<span data-ttu-id="6745c-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="6745c-123">OMA.</span></span> <span data-ttu-id="6745c-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6745c-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="6745c-125">値</span><span class="sxs-lookup"><span data-stu-id="6745c-125">value</span></span>|<span data-ttu-id="6745c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="6745c-126">Int32</span></span>|<span data-ttu-id="6745c-127">値。</span><span class="sxs-lookup"><span data-stu-id="6745c-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6745c-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6745c-128">Relationships</span></span>
<span data-ttu-id="6745c-129">なし</span><span class="sxs-lookup"><span data-stu-id="6745c-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6745c-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6745c-130">JSON Representation</span></span>
<span data-ttu-id="6745c-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6745c-131">Here is a JSON representation of the resource.</span></span>
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





