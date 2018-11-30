---
title: windowsDeviceADAccount リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: f1318f22c9bbb4b89779ddbdf130efbc6b01a7cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070314"
---
# <a name="windowsdeviceadaccount-resource-type"></a><span data-ttu-id="d24fe-103">windowsDeviceADAccount リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d24fe-103">windowsDeviceADAccount resource type</span></span>

> <span data-ttu-id="d24fe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d24fe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d24fe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d24fe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d24fe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d24fe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d24fe-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d24fe-107">Not yet documented</span></span>

<span data-ttu-id="d24fe-108">[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d24fe-108">Inherits from [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d24fe-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d24fe-109">Properties</span></span>
|<span data-ttu-id="d24fe-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d24fe-110">Property</span></span>|<span data-ttu-id="d24fe-111">型</span><span class="sxs-lookup"><span data-stu-id="d24fe-111">Type</span></span>|<span data-ttu-id="d24fe-112">説明</span><span class="sxs-lookup"><span data-stu-id="d24fe-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d24fe-113">password</span><span class="sxs-lookup"><span data-stu-id="d24fe-113">password</span></span>|<span data-ttu-id="d24fe-114">文字列</span><span class="sxs-lookup"><span data-stu-id="d24fe-114">String</span></span>|<span data-ttu-id="d24fe-115">まだ文書化されていない。[windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d24fe-115">Not yet documented Inherited from [windowsDeviceAccount](../resources/intune-devices-windowsdeviceaccount.md)</span></span>|
|<span data-ttu-id="d24fe-116">domainName</span><span class="sxs-lookup"><span data-stu-id="d24fe-116">domainName</span></span>|<span data-ttu-id="d24fe-117">String</span><span class="sxs-lookup"><span data-stu-id="d24fe-117">String</span></span>|<span data-ttu-id="d24fe-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d24fe-118">Not yet documented</span></span>|
|<span data-ttu-id="d24fe-119">userName</span><span class="sxs-lookup"><span data-stu-id="d24fe-119">userName</span></span>|<span data-ttu-id="d24fe-120">String</span><span class="sxs-lookup"><span data-stu-id="d24fe-120">String</span></span>|<span data-ttu-id="d24fe-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d24fe-121">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="d24fe-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d24fe-122">Relationships</span></span>
<span data-ttu-id="d24fe-123">なし</span><span class="sxs-lookup"><span data-stu-id="d24fe-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d24fe-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d24fe-124">JSON Representation</span></span>
<span data-ttu-id="d24fe-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d24fe-125">Here is a JSON representation of the resource.</span></span>
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





