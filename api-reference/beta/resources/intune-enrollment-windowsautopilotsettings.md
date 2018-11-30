---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。
ms.openlocfilehash: 41caab7578be08a56ecad94bbae11c43945037c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070517"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="86aa3-103">windowsAutopilotSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="86aa3-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="86aa3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86aa3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86aa3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86aa3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="86aa3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="86aa3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="86aa3-107">WindowsAutopilotSettings リソースは、Windows デバイスのデータの同期サービスを使用してデータを同期する Windows 自動操縦のアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-107">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>
## <a name="methods"></a><span data-ttu-id="86aa3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="86aa3-108">Methods</span></span>
|<span data-ttu-id="86aa3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="86aa3-109">Method</span></span>|<span data-ttu-id="86aa3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="86aa3-110">Return Type</span></span>|<span data-ttu-id="86aa3-111">説明</span><span class="sxs-lookup"><span data-stu-id="86aa3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="86aa3-112">WindowsAutopilotSettings を取得します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-112">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="86aa3-113">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="86aa3-113">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="86aa3-114">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86aa3-114">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="86aa3-115">WindowsAutopilotSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-115">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="86aa3-116">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="86aa3-116">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="86aa3-117">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-117">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="86aa3-118">同期アクション</span><span class="sxs-lookup"><span data-stu-id="86aa3-118">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="86aa3-119">なし</span><span class="sxs-lookup"><span data-stu-id="86aa3-119">None</span></span>|<span data-ttu-id="86aa3-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="86aa3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="86aa3-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86aa3-121">Properties</span></span>
|<span data-ttu-id="86aa3-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="86aa3-122">Property</span></span>|<span data-ttu-id="86aa3-123">型</span><span class="sxs-lookup"><span data-stu-id="86aa3-123">Type</span></span>|<span data-ttu-id="86aa3-124">説明</span><span class="sxs-lookup"><span data-stu-id="86aa3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86aa3-125">id</span><span class="sxs-lookup"><span data-stu-id="86aa3-125">id</span></span>|<span data-ttu-id="86aa3-126">String</span><span class="sxs-lookup"><span data-stu-id="86aa3-126">String</span></span>|<span data-ttu-id="86aa3-127">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="86aa3-127">The GUID for the object</span></span>|
|<span data-ttu-id="86aa3-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="86aa3-128">lastSyncDateTime</span></span>|<span data-ttu-id="86aa3-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86aa3-129">DateTimeOffset</span></span>|<span data-ttu-id="86aa3-130">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-130">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="86aa3-131">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="86aa3-131">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="86aa3-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="86aa3-132">DateTimeOffset</span></span>|<span data-ttu-id="86aa3-133">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-133">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="86aa3-134">syncStatus</span><span class="sxs-lookup"><span data-stu-id="86aa3-134">syncStatus</span></span>|[<span data-ttu-id="86aa3-135">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="86aa3-135">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="86aa3-136">デバイスのデータ同期 (DDS) のサービスとの同期のステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="86aa3-136">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="86aa3-137">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="86aa3-137">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="86aa3-138">関係</span><span class="sxs-lookup"><span data-stu-id="86aa3-138">Relationships</span></span>
<span data-ttu-id="86aa3-139">なし</span><span class="sxs-lookup"><span data-stu-id="86aa3-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="86aa3-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="86aa3-140">JSON Representation</span></span>
<span data-ttu-id="86aa3-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="86aa3-141">Here is a JSON representation of the resource.</span></span>
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





