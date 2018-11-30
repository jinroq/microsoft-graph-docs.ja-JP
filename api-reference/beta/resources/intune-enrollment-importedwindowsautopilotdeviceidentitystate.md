---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
ms.openlocfilehash: cdb13df520d109ddcc49e2637652499186ac9f24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071312"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="6a556-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6a556-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="6a556-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6a556-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a556-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a556-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6a556-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6a556-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a556-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6a556-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6a556-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a556-108">Properties</span></span>
|<span data-ttu-id="6a556-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a556-109">Property</span></span>|<span data-ttu-id="6a556-110">型</span><span class="sxs-lookup"><span data-stu-id="6a556-110">Type</span></span>|<span data-ttu-id="6a556-111">説明</span><span class="sxs-lookup"><span data-stu-id="6a556-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a556-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="6a556-112">deviceImportStatus</span></span>|[<span data-ttu-id="6a556-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="6a556-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="6a556-114">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="6a556-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="6a556-115">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="6a556-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="6a556-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="6a556-116">deviceRegistrationId</span></span>|<span data-ttu-id="6a556-117">String</span><span class="sxs-lookup"><span data-stu-id="6a556-117">String</span></span>|<span data-ttu-id="6a556-118">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="6a556-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="6a556-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="6a556-119">deviceErrorCode</span></span>|<span data-ttu-id="6a556-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6a556-120">Int32</span></span>|<span data-ttu-id="6a556-121">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="6a556-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="6a556-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="6a556-122">deviceErrorName</span></span>|<span data-ttu-id="6a556-123">String</span><span class="sxs-lookup"><span data-stu-id="6a556-123">String</span></span>|<span data-ttu-id="6a556-124">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="6a556-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a556-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6a556-125">Relationships</span></span>
<span data-ttu-id="6a556-126">なし</span><span class="sxs-lookup"><span data-stu-id="6a556-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6a556-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6a556-127">JSON Representation</span></span>
<span data-ttu-id="6a556-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6a556-128">Here is a JSON representation of the resource.</span></span>
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





