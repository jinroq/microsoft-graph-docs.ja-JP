---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: b8df80f71e6767e22a35db2d82a18e0a7263342d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304509"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="315b4-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="315b4-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="315b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="315b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="315b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="315b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="315b4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="315b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="315b4-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="315b4-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="315b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="315b4-108">Properties</span></span>
|<span data-ttu-id="315b4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="315b4-109">Property</span></span>|<span data-ttu-id="315b4-110">種類</span><span class="sxs-lookup"><span data-stu-id="315b4-110">Type</span></span>|<span data-ttu-id="315b4-111">説明</span><span class="sxs-lookup"><span data-stu-id="315b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="315b4-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="315b4-112">deviceImportStatus</span></span>|[<span data-ttu-id="315b4-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="315b4-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="315b4-114">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="315b4-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="315b4-115">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="315b4-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="315b4-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="315b4-116">deviceRegistrationId</span></span>|<span data-ttu-id="315b4-117">String</span><span class="sxs-lookup"><span data-stu-id="315b4-117">String</span></span>|<span data-ttu-id="315b4-118">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="315b4-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="315b4-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="315b4-119">deviceErrorCode</span></span>|<span data-ttu-id="315b4-120">Int32</span><span class="sxs-lookup"><span data-stu-id="315b4-120">Int32</span></span>|<span data-ttu-id="315b4-121">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="315b4-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="315b4-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="315b4-122">deviceErrorName</span></span>|<span data-ttu-id="315b4-123">String</span><span class="sxs-lookup"><span data-stu-id="315b4-123">String</span></span>|<span data-ttu-id="315b4-124">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="315b4-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="315b4-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="315b4-125">Relationships</span></span>
<span data-ttu-id="315b4-126">なし</span><span class="sxs-lookup"><span data-stu-id="315b4-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="315b4-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="315b4-127">JSON Representation</span></span>
<span data-ttu-id="315b4-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="315b4-128">Here is a JSON representation of the resource.</span></span>
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





