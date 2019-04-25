---
title: updateWindowsDeviceAccountActionParameter リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d67599dfc9db2afa337324e3f1ba9334134458f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523309"
---
# <a name="updatewindowsdeviceaccountactionparameter-resource-type"></a><span data-ttu-id="86936-103">updateWindowsDeviceAccountActionParameter リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86936-103">updateWindowsDeviceAccountActionParameter resource type</span></span>

> <span data-ttu-id="86936-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86936-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86936-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="86936-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86936-106">Properties</span></span>
|<span data-ttu-id="86936-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86936-107">Property</span></span>|<span data-ttu-id="86936-108">型</span><span class="sxs-lookup"><span data-stu-id="86936-108">Type</span></span>|<span data-ttu-id="86936-109">説明</span><span class="sxs-lookup"><span data-stu-id="86936-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86936-110">deviceAccount</span><span class="sxs-lookup"><span data-stu-id="86936-110">deviceAccount</span></span>|[<span data-ttu-id="86936-111">windowsDeviceAccount</span><span class="sxs-lookup"><span data-stu-id="86936-111">windowsDeviceAccount</span></span>](../resources/intune-devices-windowsdeviceaccount.md)|<span data-ttu-id="86936-112">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-112">Not yet documented</span></span>|
|<span data-ttu-id="86936-113">passwordRotationEnabled</span><span class="sxs-lookup"><span data-stu-id="86936-113">passwordRotationEnabled</span></span>|<span data-ttu-id="86936-114">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="86936-114">Boolean</span></span>|<span data-ttu-id="86936-115">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-115">Not yet documented</span></span>|
|<span data-ttu-id="86936-116">calendarSyncEnabled</span><span class="sxs-lookup"><span data-stu-id="86936-116">calendarSyncEnabled</span></span>|<span data-ttu-id="86936-117">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="86936-117">Boolean</span></span>|<span data-ttu-id="86936-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-118">Not yet documented</span></span>|
|<span data-ttu-id="86936-119">deviceAccountEmail</span><span class="sxs-lookup"><span data-stu-id="86936-119">deviceAccountEmail</span></span>|<span data-ttu-id="86936-120">String</span><span class="sxs-lookup"><span data-stu-id="86936-120">String</span></span>|<span data-ttu-id="86936-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-121">Not yet documented</span></span>|
|<span data-ttu-id="86936-122">exchangeServer</span><span class="sxs-lookup"><span data-stu-id="86936-122">exchangeServer</span></span>|<span data-ttu-id="86936-123">String</span><span class="sxs-lookup"><span data-stu-id="86936-123">String</span></span>|<span data-ttu-id="86936-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-124">Not yet documented</span></span>|
|<span data-ttu-id="86936-125">sessionInitiationProtocalAddress</span><span class="sxs-lookup"><span data-stu-id="86936-125">sessionInitiationProtocalAddress</span></span>|<span data-ttu-id="86936-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="86936-126">String</span></span>|<span data-ttu-id="86936-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86936-127">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="86936-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="86936-128">Relationships</span></span>
<span data-ttu-id="86936-129">なし</span><span class="sxs-lookup"><span data-stu-id="86936-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="86936-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86936-130">JSON Representation</span></span>
<span data-ttu-id="86936-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86936-131">Here is a JSON representation of the resource.</span></span>
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



