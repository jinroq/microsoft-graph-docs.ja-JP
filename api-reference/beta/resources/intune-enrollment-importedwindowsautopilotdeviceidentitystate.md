---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f392f011f4bfcc615f88b6ea965fbc2b47899c9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941536"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="8e1fd-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8e1fd-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="8e1fd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e1fd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e1fd-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8e1fd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8e1fd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e1fd-107">Properties</span></span>
|<span data-ttu-id="8e1fd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e1fd-108">Property</span></span>|<span data-ttu-id="8e1fd-109">型</span><span class="sxs-lookup"><span data-stu-id="8e1fd-109">Type</span></span>|<span data-ttu-id="8e1fd-110">説明</span><span class="sxs-lookup"><span data-stu-id="8e1fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e1fd-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="8e1fd-111">deviceImportStatus</span></span>|[<span data-ttu-id="8e1fd-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="8e1fd-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="8e1fd-113">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="8e1fd-114">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="8e1fd-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="8e1fd-115">deviceRegistrationId</span></span>|<span data-ttu-id="8e1fd-116">String</span><span class="sxs-lookup"><span data-stu-id="8e1fd-116">String</span></span>|<span data-ttu-id="8e1fd-117">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8e1fd-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="8e1fd-118">deviceErrorCode</span></span>|<span data-ttu-id="8e1fd-119">Int32</span><span class="sxs-lookup"><span data-stu-id="8e1fd-119">Int32</span></span>|<span data-ttu-id="8e1fd-120">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8e1fd-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="8e1fd-121">deviceErrorName</span></span>|<span data-ttu-id="8e1fd-122">String</span><span class="sxs-lookup"><span data-stu-id="8e1fd-122">String</span></span>|<span data-ttu-id="8e1fd-123">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e1fd-124">関係</span><span class="sxs-lookup"><span data-stu-id="8e1fd-124">Relationships</span></span>
<span data-ttu-id="8e1fd-125">なし</span><span class="sxs-lookup"><span data-stu-id="8e1fd-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e1fd-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8e1fd-126">JSON Representation</span></span>
<span data-ttu-id="8e1fd-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8e1fd-127">Here is a JSON representation of the resource.</span></span>
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




