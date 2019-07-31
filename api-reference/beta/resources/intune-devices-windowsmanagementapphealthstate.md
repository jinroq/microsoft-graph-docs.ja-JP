---
title: windowsManagementAppHealthState リソースの種類
description: Windows management アプリの正常性状態エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bcd116b4b5f5bc9748d16a202ea0dc2a4485299
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999375"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="57e69-103">windowsManagementAppHealthState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57e69-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="57e69-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57e69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57e69-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="57e69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57e69-106">Windows management アプリの正常性状態エンティティ。</span><span class="sxs-lookup"><span data-stu-id="57e69-106">Windows management app health state entity.</span></span>

## <a name="methods"></a><span data-ttu-id="57e69-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="57e69-107">Methods</span></span>
|<span data-ttu-id="57e69-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="57e69-108">Method</span></span>|<span data-ttu-id="57e69-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="57e69-109">Return Type</span></span>|<span data-ttu-id="57e69-110">説明</span><span class="sxs-lookup"><span data-stu-id="57e69-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="57e69-111">リスト windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="57e69-111">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="57e69-112">[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="57e69-112">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="57e69-113">[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="57e69-113">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="57e69-114">WindowsManagementAppHealthState を取得する</span><span class="sxs-lookup"><span data-stu-id="57e69-114">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="57e69-115">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="57e69-115">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="57e69-116">[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="57e69-116">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="57e69-117">WindowsManagementAppHealthState を作成する</span><span class="sxs-lookup"><span data-stu-id="57e69-117">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="57e69-118">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="57e69-118">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="57e69-119">新しい[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="57e69-119">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="57e69-120">WindowsManagementAppHealthState の削除</span><span class="sxs-lookup"><span data-stu-id="57e69-120">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="57e69-121">None</span><span class="sxs-lookup"><span data-stu-id="57e69-121">None</span></span>|<span data-ttu-id="57e69-122">[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="57e69-122">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="57e69-123">WindowsManagementAppHealthState を更新する</span><span class="sxs-lookup"><span data-stu-id="57e69-123">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="57e69-124">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="57e69-124">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="57e69-125">[Windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57e69-125">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="57e69-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e69-126">Properties</span></span>
|<span data-ttu-id="57e69-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e69-127">Property</span></span>|<span data-ttu-id="57e69-128">型</span><span class="sxs-lookup"><span data-stu-id="57e69-128">Type</span></span>|<span data-ttu-id="57e69-129">説明</span><span class="sxs-lookup"><span data-stu-id="57e69-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e69-130">id</span><span class="sxs-lookup"><span data-stu-id="57e69-130">id</span></span>|<span data-ttu-id="57e69-131">String</span><span class="sxs-lookup"><span data-stu-id="57e69-131">String</span></span>|<span data-ttu-id="57e69-132">Windows management アプリの正常性状態の一意識別子</span><span class="sxs-lookup"><span data-stu-id="57e69-132">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="57e69-133">healthState</span><span class="sxs-lookup"><span data-stu-id="57e69-133">healthState</span></span>|[<span data-ttu-id="57e69-134">healthState</span><span class="sxs-lookup"><span data-stu-id="57e69-134">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="57e69-135">Windows management アプリの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="57e69-135">Windows management app health state.</span></span> <span data-ttu-id="57e69-136">可能な値は、`unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="57e69-136">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="57e69-137">バージョン</span><span class="sxs-lookup"><span data-stu-id="57e69-137">installedVersion</span></span>|<span data-ttu-id="57e69-138">String</span><span class="sxs-lookup"><span data-stu-id="57e69-138">String</span></span>|<span data-ttu-id="57e69-139">Windows management アプリがインストールされているバージョン。</span><span class="sxs-lookup"><span data-stu-id="57e69-139">Windows management app installed version.</span></span>|
|<span data-ttu-id="57e69-140">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="57e69-140">lastCheckInDateTime</span></span>|<span data-ttu-id="57e69-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57e69-141">DateTimeOffset</span></span>|<span data-ttu-id="57e69-142">Windows management アプリの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="57e69-142">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="57e69-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="57e69-143">deviceName</span></span>|<span data-ttu-id="57e69-144">String</span><span class="sxs-lookup"><span data-stu-id="57e69-144">String</span></span>|<span data-ttu-id="57e69-145">Windows management アプリがインストールされているデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="57e69-145">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="57e69-146">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="57e69-146">deviceOSVersion</span></span>|<span data-ttu-id="57e69-147">String</span><span class="sxs-lookup"><span data-stu-id="57e69-147">String</span></span>|<span data-ttu-id="57e69-148">Windows 管理アプリがインストールされているデバイスの windows 10 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="57e69-148">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57e69-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="57e69-149">Relationships</span></span>
<span data-ttu-id="57e69-150">なし</span><span class="sxs-lookup"><span data-stu-id="57e69-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57e69-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57e69-151">JSON Representation</span></span>
<span data-ttu-id="57e69-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="57e69-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```





