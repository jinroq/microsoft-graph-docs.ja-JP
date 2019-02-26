---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261706"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="2692c-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2692c-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="2692c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2692c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2692c-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2692c-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2692c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2692c-106">Properties</span></span>
|<span data-ttu-id="2692c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2692c-107">Property</span></span>|<span data-ttu-id="2692c-108">型</span><span class="sxs-lookup"><span data-stu-id="2692c-108">Type</span></span>|<span data-ttu-id="2692c-109">説明</span><span class="sxs-lookup"><span data-stu-id="2692c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2692c-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="2692c-110">deviceImportStatus</span></span>|[<span data-ttu-id="2692c-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="2692c-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="2692c-112">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="2692c-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="2692c-113">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="2692c-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="2692c-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="2692c-114">deviceRegistrationId</span></span>|<span data-ttu-id="2692c-115">String</span><span class="sxs-lookup"><span data-stu-id="2692c-115">String</span></span>|<span data-ttu-id="2692c-116">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="2692c-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2692c-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="2692c-117">deviceErrorCode</span></span>|<span data-ttu-id="2692c-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2692c-118">Int32</span></span>|<span data-ttu-id="2692c-119">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="2692c-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2692c-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="2692c-120">deviceErrorName</span></span>|<span data-ttu-id="2692c-121">String</span><span class="sxs-lookup"><span data-stu-id="2692c-121">String</span></span>|<span data-ttu-id="2692c-122">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="2692c-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2692c-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2692c-123">Relationships</span></span>
<span data-ttu-id="2692c-124">なし</span><span class="sxs-lookup"><span data-stu-id="2692c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2692c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2692c-125">JSON Representation</span></span>
<span data-ttu-id="2692c-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2692c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



