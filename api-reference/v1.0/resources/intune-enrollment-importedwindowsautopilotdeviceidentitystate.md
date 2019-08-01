---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01524085500f8c8f8b313a9b2fbcbb89134de594
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030619"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="7cd41-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7cd41-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="7cd41-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7cd41-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cd41-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7cd41-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7cd41-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cd41-106">Properties</span></span>
|<span data-ttu-id="7cd41-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7cd41-107">Property</span></span>|<span data-ttu-id="7cd41-108">型</span><span class="sxs-lookup"><span data-stu-id="7cd41-108">Type</span></span>|<span data-ttu-id="7cd41-109">説明</span><span class="sxs-lookup"><span data-stu-id="7cd41-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cd41-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="7cd41-110">deviceImportStatus</span></span>|[<span data-ttu-id="7cd41-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="7cd41-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="7cd41-112">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="7cd41-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="7cd41-113">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="7cd41-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="7cd41-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="7cd41-114">deviceRegistrationId</span></span>|<span data-ttu-id="7cd41-115">String</span><span class="sxs-lookup"><span data-stu-id="7cd41-115">String</span></span>|<span data-ttu-id="7cd41-116">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="7cd41-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="7cd41-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="7cd41-117">deviceErrorCode</span></span>|<span data-ttu-id="7cd41-118">Int32</span><span class="sxs-lookup"><span data-stu-id="7cd41-118">Int32</span></span>|<span data-ttu-id="7cd41-119">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="7cd41-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="7cd41-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="7cd41-120">deviceErrorName</span></span>|<span data-ttu-id="7cd41-121">String</span><span class="sxs-lookup"><span data-stu-id="7cd41-121">String</span></span>|<span data-ttu-id="7cd41-122">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="7cd41-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7cd41-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7cd41-123">Relationships</span></span>
<span data-ttu-id="7cd41-124">なし</span><span class="sxs-lookup"><span data-stu-id="7cd41-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7cd41-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7cd41-125">JSON Representation</span></span>
<span data-ttu-id="7cd41-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7cd41-126">Here is a JSON representation of the resource.</span></span>
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



