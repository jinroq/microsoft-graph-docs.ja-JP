---
title: importedWindowsAutopilotDeviceIdentityState リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b8130c354157bcfe679a95914e9266e500a6b51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972944"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="12cbc-103">importedWindowsAutopilotDeviceIdentityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12cbc-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="12cbc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="12cbc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="12cbc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12cbc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12cbc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="12cbc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="12cbc-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="12cbc-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="12cbc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12cbc-108">Properties</span></span>
|<span data-ttu-id="12cbc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12cbc-109">Property</span></span>|<span data-ttu-id="12cbc-110">種類</span><span class="sxs-lookup"><span data-stu-id="12cbc-110">Type</span></span>|<span data-ttu-id="12cbc-111">説明</span><span class="sxs-lookup"><span data-stu-id="12cbc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cbc-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="12cbc-112">deviceImportStatus</span></span>|[<span data-ttu-id="12cbc-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="12cbc-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="12cbc-114">Device Directory Service (DDS) から報告されたデバイスの状態です。</span><span class="sxs-lookup"><span data-stu-id="12cbc-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="12cbc-115">可能な値は、`unknown`、`pending`、`partial`、`complete`、`error` です。</span><span class="sxs-lookup"><span data-stu-id="12cbc-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="12cbc-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="12cbc-116">deviceRegistrationId</span></span>|<span data-ttu-id="12cbc-117">String</span><span class="sxs-lookup"><span data-stu-id="12cbc-117">String</span></span>|<span data-ttu-id="12cbc-118">正常に追加されたと Devce Directory Service (DDS) から報告されたデバイスの Devce Registration ID です。</span><span class="sxs-lookup"><span data-stu-id="12cbc-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="12cbc-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="12cbc-119">deviceErrorCode</span></span>|<span data-ttu-id="12cbc-120">Int32</span><span class="sxs-lookup"><span data-stu-id="12cbc-120">Int32</span></span>|<span data-ttu-id="12cbc-121">Device Directory Service (DDS) から報告されたデバイス エラー コードです。</span><span class="sxs-lookup"><span data-stu-id="12cbc-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="12cbc-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="12cbc-122">deviceErrorName</span></span>|<span data-ttu-id="12cbc-123">String</span><span class="sxs-lookup"><span data-stu-id="12cbc-123">String</span></span>|<span data-ttu-id="12cbc-124">Device Directory Service (DDS) から報告されたデバイス エラー名です。</span><span class="sxs-lookup"><span data-stu-id="12cbc-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="12cbc-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12cbc-125">Relationships</span></span>
<span data-ttu-id="12cbc-126">なし</span><span class="sxs-lookup"><span data-stu-id="12cbc-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="12cbc-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12cbc-127">JSON Representation</span></span>
<span data-ttu-id="12cbc-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12cbc-128">Here is a JSON representation of the resource.</span></span>
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





