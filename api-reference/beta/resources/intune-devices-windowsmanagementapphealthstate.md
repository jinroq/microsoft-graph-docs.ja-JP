---
title: windowsmanagementapphealthstate リソースの種類
description: Windows management アプリの正常性状態エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8841b79b9a284a15999db701e82a2b5062e2930b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148539"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="5f1cb-103">windowsmanagementapphealthstate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5f1cb-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="5f1cb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f1cb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f1cb-106">Windows management アプリの正常性状態エンティティ。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-106">Windows management app health state entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5f1cb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f1cb-107">Methods</span></span>
|<span data-ttu-id="5f1cb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5f1cb-108">Method</span></span>|<span data-ttu-id="5f1cb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5f1cb-109">Return Type</span></span>|<span data-ttu-id="5f1cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="5f1cb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5f1cb-111">リスト windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="5f1cb-111">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="5f1cb-112">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5f1cb-112">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="5f1cb-113">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-113">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="5f1cb-114">windowsmanagementapphealthstate を取得する</span><span class="sxs-lookup"><span data-stu-id="5f1cb-114">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="5f1cb-115">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="5f1cb-115">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="5f1cb-116">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-116">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="5f1cb-117">windowsmanagementapphealthstate を作成する</span><span class="sxs-lookup"><span data-stu-id="5f1cb-117">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="5f1cb-118">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="5f1cb-118">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="5f1cb-119">新しい[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-119">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="5f1cb-120">windowsmanagementapphealthstate の削除</span><span class="sxs-lookup"><span data-stu-id="5f1cb-120">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="5f1cb-121">なし</span><span class="sxs-lookup"><span data-stu-id="5f1cb-121">None</span></span>|<span data-ttu-id="5f1cb-122">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-122">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="5f1cb-123">windowsmanagementapphealthstate を更新する</span><span class="sxs-lookup"><span data-stu-id="5f1cb-123">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="5f1cb-124">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="5f1cb-124">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="5f1cb-125">[windowsmanagementapphealthstate](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-125">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5f1cb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f1cb-126">Properties</span></span>
|<span data-ttu-id="5f1cb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f1cb-127">Property</span></span>|<span data-ttu-id="5f1cb-128">型</span><span class="sxs-lookup"><span data-stu-id="5f1cb-128">Type</span></span>|<span data-ttu-id="5f1cb-129">説明</span><span class="sxs-lookup"><span data-stu-id="5f1cb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f1cb-130">id</span><span class="sxs-lookup"><span data-stu-id="5f1cb-130">id</span></span>|<span data-ttu-id="5f1cb-131">文字列</span><span class="sxs-lookup"><span data-stu-id="5f1cb-131">String</span></span>|<span data-ttu-id="5f1cb-132">Windows management アプリの正常性状態の一意識別子</span><span class="sxs-lookup"><span data-stu-id="5f1cb-132">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="5f1cb-133">healthState</span><span class="sxs-lookup"><span data-stu-id="5f1cb-133">healthState</span></span>|[<span data-ttu-id="5f1cb-134">healthState</span><span class="sxs-lookup"><span data-stu-id="5f1cb-134">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="5f1cb-135">Windows management アプリの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-135">Windows management app health state.</span></span> <span data-ttu-id="5f1cb-136">可能な値は `unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-136">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="5f1cb-137">バージョン</span><span class="sxs-lookup"><span data-stu-id="5f1cb-137">installedVersion</span></span>|<span data-ttu-id="5f1cb-138">String</span><span class="sxs-lookup"><span data-stu-id="5f1cb-138">String</span></span>|<span data-ttu-id="5f1cb-139">Windows management アプリがインストールされているバージョン。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-139">Windows management app installed version.</span></span>|
|<span data-ttu-id="5f1cb-140">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="5f1cb-140">lastCheckInDateTime</span></span>|<span data-ttu-id="5f1cb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5f1cb-141">DateTimeOffset</span></span>|<span data-ttu-id="5f1cb-142">Windows management アプリの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-142">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="5f1cb-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="5f1cb-143">deviceName</span></span>|<span data-ttu-id="5f1cb-144">String</span><span class="sxs-lookup"><span data-stu-id="5f1cb-144">String</span></span>|<span data-ttu-id="5f1cb-145">Windows management アプリがインストールされているデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-145">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="5f1cb-146">deviceosversion</span><span class="sxs-lookup"><span data-stu-id="5f1cb-146">deviceOSVersion</span></span>|<span data-ttu-id="5f1cb-147">String</span><span class="sxs-lookup"><span data-stu-id="5f1cb-147">String</span></span>|<span data-ttu-id="5f1cb-148">windows 管理アプリがインストールされているデバイスの windows 10 OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-148">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f1cb-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5f1cb-149">Relationships</span></span>
<span data-ttu-id="5f1cb-150">なし</span><span class="sxs-lookup"><span data-stu-id="5f1cb-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f1cb-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5f1cb-151">JSON Representation</span></span>
<span data-ttu-id="5f1cb-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5f1cb-152">Here is a JSON representation of the resource.</span></span>
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




