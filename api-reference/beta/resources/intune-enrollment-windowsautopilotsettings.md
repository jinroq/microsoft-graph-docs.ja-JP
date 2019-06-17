---
title: windowsAutopilotSettings リソースの種類
description: WindowsAutopilotSettings リソースは、windows device data sync service とデータを同期する Windows 自動操縦アカウントを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7bbdfa28061b48a0c2ca3ed2e0b714e1f1a1159
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989715"
---
# <a name="windowsautopilotsettings-resource-type"></a><span data-ttu-id="7f2f6-103">windowsAutopilotSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f2f6-103">windowsAutopilotSettings resource type</span></span>

> <span data-ttu-id="7f2f6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f2f6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f2f6-106">WindowsAutopilotSettings リソースは、windows device data sync service とデータを同期する Windows 自動操縦アカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-106">The windowsAutopilotSettings resource represents a Windows Autopilot Account to sync data with Windows device data sync service.</span></span>

## <a name="methods"></a><span data-ttu-id="7f2f6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f2f6-107">Methods</span></span>
|<span data-ttu-id="7f2f6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f2f6-108">Method</span></span>|<span data-ttu-id="7f2f6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f2f6-109">Return Type</span></span>|<span data-ttu-id="7f2f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="7f2f6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f2f6-111">WindowsAutopilotSettings を取得する</span><span class="sxs-lookup"><span data-stu-id="7f2f6-111">Get windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-get.md)|[<span data-ttu-id="7f2f6-112">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="7f2f6-112">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="7f2f6-113">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-113">Read properties and relationships of the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="7f2f6-114">WindowsAutopilotSettings の更新</span><span class="sxs-lookup"><span data-stu-id="7f2f6-114">Update windowsAutopilotSettings</span></span>](../api/intune-enrollment-windowsautopilotsettings-update.md)|[<span data-ttu-id="7f2f6-115">windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="7f2f6-115">windowsAutopilotSettings</span></span>](../resources/intune-enrollment-windowsautopilotsettings.md)|<span data-ttu-id="7f2f6-116">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-116">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>|
|[<span data-ttu-id="7f2f6-117">同期アクション</span><span class="sxs-lookup"><span data-stu-id="7f2f6-117">sync action</span></span>](../api/intune-enrollment-windowsautopilotsettings-sync.md)|<span data-ttu-id="7f2f6-118">なし</span><span class="sxs-lookup"><span data-stu-id="7f2f6-118">None</span></span>|<span data-ttu-id="7f2f6-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7f2f6-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7f2f6-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f2f6-120">Properties</span></span>
|<span data-ttu-id="7f2f6-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f2f6-121">Property</span></span>|<span data-ttu-id="7f2f6-122">型</span><span class="sxs-lookup"><span data-stu-id="7f2f6-122">Type</span></span>|<span data-ttu-id="7f2f6-123">説明</span><span class="sxs-lookup"><span data-stu-id="7f2f6-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f2f6-124">id</span><span class="sxs-lookup"><span data-stu-id="7f2f6-124">id</span></span>|<span data-ttu-id="7f2f6-125">String</span><span class="sxs-lookup"><span data-stu-id="7f2f6-125">String</span></span>|<span data-ttu-id="7f2f6-126">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="7f2f6-126">The GUID for the object</span></span>|
|<span data-ttu-id="7f2f6-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="7f2f6-127">lastSyncDateTime</span></span>|<span data-ttu-id="7f2f6-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f2f6-128">DateTimeOffset</span></span>|<span data-ttu-id="7f2f6-129">DDS サービスによる最終データ同期日時。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-129">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="7f2f6-130">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="7f2f6-130">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="7f2f6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f2f6-131">DateTimeOffset</span></span>|<span data-ttu-id="7f2f6-132">DDS サービスによる最終データ同期日時。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-132">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="7f2f6-133">syncStatus</span><span class="sxs-lookup"><span data-stu-id="7f2f6-133">syncStatus</span></span>|[<span data-ttu-id="7f2f6-134">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="7f2f6-134">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="7f2f6-135">デバイスデータ同期 (DDS) サービスとの同期の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-135">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="7f2f6-136">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-136">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f2f6-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f2f6-137">Relationships</span></span>
<span data-ttu-id="7f2f6-138">なし</span><span class="sxs-lookup"><span data-stu-id="7f2f6-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f2f6-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f2f6-139">JSON Representation</span></span>
<span data-ttu-id="7f2f6-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f2f6-140">Here is a JSON representation of the resource.</span></span>
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





