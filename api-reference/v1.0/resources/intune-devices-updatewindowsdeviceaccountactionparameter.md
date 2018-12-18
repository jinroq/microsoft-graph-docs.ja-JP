---
title: updateWindowsDeviceAccountActionParameter リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: cd69ffa01473a40228d53ad2f68f793cadf838d5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27335463"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="124de-103">updateWindowsDeviceAccountActionParameter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="124de-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="124de-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="124de-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="124de-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="124de-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="124de-106">Properties</span></span>
|<span data-ttu-id="124de-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="124de-107">Property</span></span>|<span data-ttu-id="124de-108">種類</span><span class="sxs-lookup"><span data-stu-id="124de-108">Type</span></span>|<span data-ttu-id="124de-109">説明</span><span class="sxs-lookup"><span data-stu-id="124de-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="124de-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="124de-110">deviceAccount</span></span>|[<span data-ttu-id="124de-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="124de-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="124de-112">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-112">Not yet documented</span></span>|
|<span data-ttu-id="124de-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="124de-113">passwordRotationEnabled</span></span>|<span data-ttu-id="124de-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="124de-114">Boolean</span></span>|<span data-ttu-id="124de-115">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-115">Not yet documented</span></span>|
|<span data-ttu-id="124de-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="124de-116">calendarSyncEnabled</span></span>|<span data-ttu-id="124de-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="124de-117">Boolean</span></span>|<span data-ttu-id="124de-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-118">Not yet documented</span></span>|
|<span data-ttu-id="124de-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="124de-119">deviceAccountEmail</span></span>|<span data-ttu-id="124de-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="124de-120">String</span></span>|<span data-ttu-id="124de-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-121">Not yet documented</span></span>|
|<span data-ttu-id="124de-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="124de-122">exchangeServer</span></span>|<span data-ttu-id="124de-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="124de-123">String</span></span>|<span data-ttu-id="124de-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-124">Not yet documented</span></span>|
|<span data-ttu-id="124de-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="124de-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="124de-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="124de-126">String</span></span>|<span data-ttu-id="124de-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="124de-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="124de-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="124de-128">Relationships</span></span>
<span data-ttu-id="124de-129">なし</span><span class="sxs-lookup"><span data-stu-id="124de-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="124de-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="124de-130">JSON Representation</span></span>
<span data-ttu-id="124de-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="124de-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "deviceAccount": {
    "@odata.type": "microsoft.graph.windowsDeviceAccount",
    "password": "String"
  },
  "passwordRotationEnabled": true,
  "calendarSyncEnabled": true,
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "sessionInitiationProtocalAddress": "String"
}
```



