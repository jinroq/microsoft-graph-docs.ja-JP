---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7beb1f04efe3b43067eb1cedeed7071561265ce6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881550"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="5e3a2-103">windowsAutopilotSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e3a2-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="5e3a2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e3a2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e3a2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e3a2-107">WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>
## <a name="methods"></a><span data-ttu-id="5e3a2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5e3a2-108">Methods</span></span>
|<span data-ttu-id="5e3a2-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5e3a2-109">Method</span></span>|<span data-ttu-id="5e3a2-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5e3a2-110">Return Type</span></span>|<span data-ttu-id="5e3a2-111">説明</span><span class="sxs-lookup"><span data-stu-id="5e3a2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e3a2-112">WindowsAutopilotSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="5e3a2-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5e3a2-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="5e3a2-114">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="5e3a2-115">WindowsAutopilotSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="5e3a2-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="5e3a2-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="5e3a2-117">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="5e3a2-118">同期アクション</span><span class="sxs-lookup"><span data-stu-id="5e3a2-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="5e3a2-119">なし</span><span class="sxs-lookup"><span data-stu-id="5e3a2-119">None</span></span>|<span data-ttu-id="5e3a2-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5e3a2-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5e3a2-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e3a2-121">Properties</span></span>
|<span data-ttu-id="5e3a2-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e3a2-122">Property</span></span>|<span data-ttu-id="5e3a2-123">種類</span><span class="sxs-lookup"><span data-stu-id="5e3a2-123">Type</span></span>|<span data-ttu-id="5e3a2-124">説明</span><span class="sxs-lookup"><span data-stu-id="5e3a2-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e3a2-125">ID</span><span class="sxs-lookup"><span data-stu-id="5e3a2-125">id</span></span>|<span data-ttu-id="5e3a2-126">String</span><span class="sxs-lookup"><span data-stu-id="5e3a2-126">String</span></span>|<span data-ttu-id="5e3a2-127">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="5e3a2-127">The GUID for the object</span></span>|
|<span data-ttu-id="5e3a2-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="5e3a2-128">lastSyncDateTime</span></span>|<span data-ttu-id="5e3a2-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e3a2-129">DateTimeOffset</span></span>|<span data-ttu-id="5e3a2-130">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="5e3a2-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="5e3a2-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="5e3a2-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e3a2-132">DateTimeOffset</span></span>|<span data-ttu-id="5e3a2-133">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="5e3a2-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="5e3a2-134">syncStatus</span></span>|[<span data-ttu-id="5e3a2-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5e3a2-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="5e3a2-136">デバイスのデータ同期 (DDS) のサービスとの同期のステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="5e3a2-137">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e3a2-138">関係</span><span class="sxs-lookup"><span data-stu-id="5e3a2-138">Relationships</span></span>
<span data-ttu-id="5e3a2-139">なし</span><span class="sxs-lookup"><span data-stu-id="5e3a2-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5e3a2-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e3a2-140">JSON Representation</span></span>
<span data-ttu-id="5e3a2-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e3a2-141">Here is a JSON representation of the resource.</span></span>
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





