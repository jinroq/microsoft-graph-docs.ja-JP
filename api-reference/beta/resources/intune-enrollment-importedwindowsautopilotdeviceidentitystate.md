---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f4e76b23d4d970a9fb873326dc84f278aa2ed2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410967"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="f39e0-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f39e0-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="f39e0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f39e0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f39e0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f39e0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f39e0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f39e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f39e0-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f39e0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f39e0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f39e0-108">Properties</span></span>
|<span data-ttu-id="f39e0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f39e0-109">Property</span></span>|<span data-ttu-id="f39e0-110">型</span><span class="sxs-lookup"><span data-stu-id="f39e0-110">Type</span></span>|<span data-ttu-id="f39e0-111">説明</span><span class="sxs-lookup"><span data-stu-id="f39e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f39e0-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="f39e0-112">deviceImportStatus</span></span>|[<span data-ttu-id="f39e0-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="f39e0-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="f39e0-114">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="f39e0-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="f39e0-115">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="f39e0-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="f39e0-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f39e0-116">deviceRegistrationId</span></span>|<span data-ttu-id="f39e0-117">String</span><span class="sxs-lookup"><span data-stu-id="f39e0-117">String</span></span>|<span data-ttu-id="f39e0-118">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="f39e0-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f39e0-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="f39e0-119">deviceErrorCode</span></span>|<span data-ttu-id="f39e0-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f39e0-120">Int32</span></span>|<span data-ttu-id="f39e0-121">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="f39e0-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f39e0-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="f39e0-122">deviceErrorName</span></span>|<span data-ttu-id="f39e0-123">String</span><span class="sxs-lookup"><span data-stu-id="f39e0-123">String</span></span>|<span data-ttu-id="f39e0-124">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="f39e0-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f39e0-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f39e0-125">Relationships</span></span>
<span data-ttu-id="f39e0-126">なし</span><span class="sxs-lookup"><span data-stu-id="f39e0-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f39e0-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f39e0-127">JSON Representation</span></span>
<span data-ttu-id="f39e0-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f39e0-128">Here is a JSON representation of the resource.</span></span>
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




