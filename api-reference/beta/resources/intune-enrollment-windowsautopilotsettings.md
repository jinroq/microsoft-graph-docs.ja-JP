---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4bf9a39d6a5078362c966edde38ec98deec037b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939554"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="80fe7-103">windowsAutopilotSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="80fe7-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="80fe7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="80fe7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80fe7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80fe7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80fe7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80fe7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80fe7-107">WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>
## <a name="methods"></a><span data-ttu-id="80fe7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="80fe7-108">Methods</span></span>
|<span data-ttu-id="80fe7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="80fe7-109">Method</span></span>|<span data-ttu-id="80fe7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="80fe7-110">Return Type</span></span>|<span data-ttu-id="80fe7-111">説明</span><span class="sxs-lookup"><span data-stu-id="80fe7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="80fe7-112">WindowsAutopilotSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="80fe7-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="80fe7-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="80fe7-114">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80fe7-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="80fe7-115">WindowsAutopilotSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="80fe7-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="80fe7-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="80fe7-117">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="80fe7-118">同期アクション</span><span class="sxs-lookup"><span data-stu-id="80fe7-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="80fe7-119">なし</span><span class="sxs-lookup"><span data-stu-id="80fe7-119">None</span></span>|<span data-ttu-id="80fe7-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="80fe7-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="80fe7-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80fe7-121">Properties</span></span>
|<span data-ttu-id="80fe7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80fe7-122">Property</span></span>|<span data-ttu-id="80fe7-123">型</span><span class="sxs-lookup"><span data-stu-id="80fe7-123">Type</span></span>|<span data-ttu-id="80fe7-124">説明</span><span class="sxs-lookup"><span data-stu-id="80fe7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80fe7-125">ID</span><span class="sxs-lookup"><span data-stu-id="80fe7-125">id</span></span>|<span data-ttu-id="80fe7-126">String</span><span class="sxs-lookup"><span data-stu-id="80fe7-126">String</span></span>|<span data-ttu-id="80fe7-127">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="80fe7-127">The GUID for the object</span></span>|
|<span data-ttu-id="80fe7-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80fe7-128">lastSyncDateTime</span></span>|<span data-ttu-id="80fe7-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80fe7-129">DateTimeOffset</span></span>|<span data-ttu-id="80fe7-130">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="80fe7-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="80fe7-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="80fe7-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80fe7-132">DateTimeOffset</span></span>|<span data-ttu-id="80fe7-133">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="80fe7-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="80fe7-134">syncStatus</span></span>|[<span data-ttu-id="80fe7-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="80fe7-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="80fe7-136">デバイスのデータ同期 (DDS) のサービスとの同期のステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="80fe7-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="80fe7-137">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="80fe7-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80fe7-138">関係</span><span class="sxs-lookup"><span data-stu-id="80fe7-138">Relationships</span></span>
<span data-ttu-id="80fe7-139">なし</span><span class="sxs-lookup"><span data-stu-id="80fe7-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80fe7-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="80fe7-140">JSON Representation</span></span>
<span data-ttu-id="80fe7-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="80fe7-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "String (identifier)",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```





