---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f6bb27b603669da82a42501563ad4be3220c7249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870764"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="2ceea-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ceea-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="2ceea-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ceea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ceea-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2ceea-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2ceea-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ceea-106">Properties</span></span>
|<span data-ttu-id="2ceea-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ceea-107">Property</span></span>|<span data-ttu-id="2ceea-108">種類</span><span class="sxs-lookup"><span data-stu-id="2ceea-108">Type</span></span>|<span data-ttu-id="2ceea-109">説明</span><span class="sxs-lookup"><span data-stu-id="2ceea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ceea-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="2ceea-110">deviceImportStatus</span></span>|[<span data-ttu-id="2ceea-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="2ceea-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="2ceea-112">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="2ceea-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="2ceea-113">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="2ceea-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="2ceea-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="2ceea-114">deviceRegistrationId</span></span>|<span data-ttu-id="2ceea-115">String</span><span class="sxs-lookup"><span data-stu-id="2ceea-115">String</span></span>|<span data-ttu-id="2ceea-116">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="2ceea-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2ceea-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="2ceea-117">deviceErrorCode</span></span>|<span data-ttu-id="2ceea-118">Int32</span><span class="sxs-lookup"><span data-stu-id="2ceea-118">Int32</span></span>|<span data-ttu-id="2ceea-119">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="2ceea-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2ceea-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="2ceea-120">deviceErrorName</span></span>|<span data-ttu-id="2ceea-121">String</span><span class="sxs-lookup"><span data-stu-id="2ceea-121">String</span></span>|<span data-ttu-id="2ceea-122">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="2ceea-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ceea-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ceea-123">Relationships</span></span>
<span data-ttu-id="2ceea-124">なし</span><span class="sxs-lookup"><span data-stu-id="2ceea-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2ceea-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ceea-125">JSON Representation</span></span>
<span data-ttu-id="2ceea-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ceea-126">Here is a JSON representation of the resource.</span></span>
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



