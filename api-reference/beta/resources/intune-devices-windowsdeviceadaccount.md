---
title: windowsDeviceADAccount リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fb421a93c1e88293758c633a08541b2f9e3ee6ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949284"
---
# <a name="windowsdeviceadaccount-resource-type"></a><span data-ttu-id="aeb4e-103">windowsDeviceADAccount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aeb4e-103">windowsDeviceADAccount resource type</span></span>

> <span data-ttu-id="aeb4e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aeb4e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aeb4e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aeb4e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aeb4e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aeb4e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aeb4e-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aeb4e-107">Not yet documented</span></span>

<span data-ttu-id="aeb4e-108">[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aeb4e-108">Inherits from [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aeb4e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aeb4e-109">Properties</span></span>
|<span data-ttu-id="aeb4e-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aeb4e-110">Property</span></span>|<span data-ttu-id="aeb4e-111">種類</span><span class="sxs-lookup"><span data-stu-id="aeb4e-111">Type</span></span>|<span data-ttu-id="aeb4e-112">説明</span><span class="sxs-lookup"><span data-stu-id="aeb4e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aeb4e-113">password</span><span class="sxs-lookup"><span data-stu-id="aeb4e-113">password</span></span>|<span data-ttu-id="aeb4e-114">文字列</span><span class="sxs-lookup"><span data-stu-id="aeb4e-114">String</span></span>|<span data-ttu-id="aeb4e-115">まだ文書化されていない。[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aeb4e-115">Not yet documented Inherited from [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)</span></span>|
|<span data-ttu-id="aeb4e-116">domainName</span><span class="sxs-lookup"><span data-stu-id="aeb4e-116">domainName</span></span>|<span data-ttu-id="aeb4e-117">String</span><span class="sxs-lookup"><span data-stu-id="aeb4e-117">String</span></span>|<span data-ttu-id="aeb4e-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aeb4e-118">Not yet documented</span></span>|
|<span data-ttu-id="aeb4e-119">userName</span><span class="sxs-lookup"><span data-stu-id="aeb4e-119">userName</span></span>|<span data-ttu-id="aeb4e-120">String</span><span class="sxs-lookup"><span data-stu-id="aeb4e-120">String</span></span>|<span data-ttu-id="aeb4e-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="aeb4e-121">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="aeb4e-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aeb4e-122">Relationships</span></span>
<span data-ttu-id="aeb4e-123">なし</span><span class="sxs-lookup"><span data-stu-id="aeb4e-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="aeb4e-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aeb4e-124">JSON Representation</span></span>
<span data-ttu-id="aeb4e-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aeb4e-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "password": "String",
  "domainName": "String",
  "userName": "String"
}
```





