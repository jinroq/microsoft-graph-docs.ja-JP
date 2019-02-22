---
title: windowsAutopilotSettings リソースの種類
description: windowsAutopilotSettings リソースは、windows device data sync service とデータを同期する windows 自動操縦アカウントを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b34d6edbed5bc98989ea70186b081d5c88a1c1b6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140517"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="c3564-103">windowsAutopilotSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c3564-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="c3564-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3564-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3564-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3564-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3564-106">windowsAutopilotSettings リソースは、windows device data sync service とデータを同期する windows 自動操縦アカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="c3564-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="c3564-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3564-107">Methods</span></span>
|<span data-ttu-id="c3564-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c3564-108">Method</span></span>|<span data-ttu-id="c3564-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c3564-109">Return Type</span></span>|<span data-ttu-id="c3564-110">説明</span><span class="sxs-lookup"><span data-stu-id="c3564-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3564-111">windowsAutopilotSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="c3564-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="c3564-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="c3564-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="c3564-113">[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c3564-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="c3564-114">windowsAutopilotSettings の更新</span><span class="sxs-lookup"><span data-stu-id="c3564-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="c3564-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="c3564-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="c3564-116">[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3564-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="c3564-117">同期アクション</span><span class="sxs-lookup"><span data-stu-id="c3564-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="c3564-118">なし</span><span class="sxs-lookup"><span data-stu-id="c3564-118">None</span></span>|<span data-ttu-id="c3564-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c3564-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c3564-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3564-120">Properties</span></span>
|<span data-ttu-id="c3564-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3564-121">Property</span></span>|<span data-ttu-id="c3564-122">型</span><span class="sxs-lookup"><span data-stu-id="c3564-122">Type</span></span>|<span data-ttu-id="c3564-123">説明</span><span class="sxs-lookup"><span data-stu-id="c3564-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3564-124">id</span><span class="sxs-lookup"><span data-stu-id="c3564-124">id</span></span>|<span data-ttu-id="c3564-125">String</span><span class="sxs-lookup"><span data-stu-id="c3564-125">String</span></span>|<span data-ttu-id="c3564-126">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="c3564-126">The GUID for the object</span></span>|
|<span data-ttu-id="c3564-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c3564-127">lastSyncDateTime</span></span>|<span data-ttu-id="c3564-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3564-128">DateTimeOffset</span></span>|<span data-ttu-id="c3564-129">DDS サービスによる最終データ同期日時。</span><span class="sxs-lookup"><span data-stu-id="c3564-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="c3564-130">lastmanualsynctriggerdatetime</span><span class="sxs-lookup"><span data-stu-id="c3564-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="c3564-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3564-131">DateTimeOffset</span></span>|<span data-ttu-id="c3564-132">DDS サービスによる最終データ同期日時。</span><span class="sxs-lookup"><span data-stu-id="c3564-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="c3564-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="c3564-133">syncStatus</span></span>|[<span data-ttu-id="c3564-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="c3564-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="c3564-135">デバイスデータ同期 (DDS) サービスとの同期の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="c3564-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="c3564-136">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="c3564-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3564-137">関係</span><span class="sxs-lookup"><span data-stu-id="c3564-137">Relationships</span></span>
<span data-ttu-id="c3564-138">なし</span><span class="sxs-lookup"><span data-stu-id="c3564-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3564-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3564-139">JSON Representation</span></span>
<span data-ttu-id="c3564-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3564-140">Here is a JSON representation of the resource.</span></span>
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




