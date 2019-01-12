---
title: windowsManagementAppHealthState リソースの種類
description: Windows 管理アプリケーションの正常性の状態エンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8cf679cf1a5ac86c47354db2fc9f800647d309c1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976472"
---
# <a name="windowsmanagementapphealthstate-resource-type"></a><span data-ttu-id="20fed-103">windowsManagementAppHealthState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20fed-103">windowsManagementAppHealthState resource type</span></span>

> <span data-ttu-id="20fed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="20fed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20fed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20fed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20fed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="20fed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20fed-107">Windows 管理アプリケーションの正常性の状態エンティティです。</span><span class="sxs-lookup"><span data-stu-id="20fed-107">Windows management app health state entity.</span></span>
## <a name="methods"></a><span data-ttu-id="20fed-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="20fed-108">Methods</span></span>
|<span data-ttu-id="20fed-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="20fed-109">Method</span></span>|<span data-ttu-id="20fed-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="20fed-110">Return Type</span></span>|<span data-ttu-id="20fed-111">説明</span><span class="sxs-lookup"><span data-stu-id="20fed-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="20fed-112">リスト windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="20fed-112">List windowsManagementAppHealthStates</span></span>](../api/intune-devices-windowsmanagementapphealthstate-list.md)|<span data-ttu-id="20fed-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="20fed-113">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="20fed-114">[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="20fed-114">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>|
|[<span data-ttu-id="20fed-115">WindowsManagementAppHealthState を取得します。</span><span class="sxs-lookup"><span data-stu-id="20fed-115">Get windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-get.md)|[<span data-ttu-id="20fed-116">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="20fed-116">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="20fed-117">[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20fed-117">Read properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="20fed-118">WindowsManagementAppHealthState を作成します。</span><span class="sxs-lookup"><span data-stu-id="20fed-118">Create windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-create.md)|[<span data-ttu-id="20fed-119">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="20fed-119">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="20fed-120">新しい[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="20fed-120">Create a new [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|
|[<span data-ttu-id="20fed-121">WindowsManagementAppHealthState を削除します。</span><span class="sxs-lookup"><span data-stu-id="20fed-121">Delete windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-delete.md)|<span data-ttu-id="20fed-122">なし</span><span class="sxs-lookup"><span data-stu-id="20fed-122">None</span></span>|<span data-ttu-id="20fed-123">の[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="20fed-123">Deletes a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md).</span></span>|
|[<span data-ttu-id="20fed-124">WindowsManagementAppHealthState を更新します。</span><span class="sxs-lookup"><span data-stu-id="20fed-124">Update windowsManagementAppHealthState</span></span>](../api/intune-devices-windowsmanagementapphealthstate-update.md)|[<span data-ttu-id="20fed-125">windowsManagementAppHealthState</span><span class="sxs-lookup"><span data-stu-id="20fed-125">windowsManagementAppHealthState</span></span>](../resources/intune-devices-windowsmanagementapphealthstate.md)|<span data-ttu-id="20fed-126">[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="20fed-126">Update the properties of a [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="20fed-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20fed-127">Properties</span></span>
|<span data-ttu-id="20fed-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20fed-128">Property</span></span>|<span data-ttu-id="20fed-129">型</span><span class="sxs-lookup"><span data-stu-id="20fed-129">Type</span></span>|<span data-ttu-id="20fed-130">説明</span><span class="sxs-lookup"><span data-stu-id="20fed-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20fed-131">ID</span><span class="sxs-lookup"><span data-stu-id="20fed-131">id</span></span>|<span data-ttu-id="20fed-132">String</span><span class="sxs-lookup"><span data-stu-id="20fed-132">String</span></span>|<span data-ttu-id="20fed-133">Windows 管理アプリケーションの正常性状態の一意の識別子</span><span class="sxs-lookup"><span data-stu-id="20fed-133">Unique Identifier for the Windows management app health state</span></span>|
|<span data-ttu-id="20fed-134">healthState</span><span class="sxs-lookup"><span data-stu-id="20fed-134">healthState</span></span>|[<span data-ttu-id="20fed-135">healthState</span><span class="sxs-lookup"><span data-stu-id="20fed-135">healthState</span></span>](../resources/intune-devices-healthstate.md)|<span data-ttu-id="20fed-136">Windows 管理アプリケーションの正常性状態。</span><span class="sxs-lookup"><span data-stu-id="20fed-136">Windows management app health state.</span></span> <span data-ttu-id="20fed-137">可能な値は、`unknown`、`healthy`、`unhealthy` です。</span><span class="sxs-lookup"><span data-stu-id="20fed-137">Possible values are: `unknown`, `healthy`, `unhealthy`.</span></span>|
|<span data-ttu-id="20fed-138">installedVersion</span><span class="sxs-lookup"><span data-stu-id="20fed-138">installedVersion</span></span>|<span data-ttu-id="20fed-139">String</span><span class="sxs-lookup"><span data-stu-id="20fed-139">String</span></span>|<span data-ttu-id="20fed-140">Windows 管理アプリケーションは、バージョンをインストールします。</span><span class="sxs-lookup"><span data-stu-id="20fed-140">Windows management app installed version.</span></span>|
|<span data-ttu-id="20fed-141">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="20fed-141">lastCheckInDateTime</span></span>|<span data-ttu-id="20fed-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20fed-142">DateTimeOffset</span></span>|<span data-ttu-id="20fed-143">Windows 管理アプリケーション最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="20fed-143">Windows management app last check-in time.</span></span>|
|<span data-ttu-id="20fed-144">deviceName</span><span class="sxs-lookup"><span data-stu-id="20fed-144">deviceName</span></span>|<span data-ttu-id="20fed-145">String</span><span class="sxs-lookup"><span data-stu-id="20fed-145">String</span></span>|<span data-ttu-id="20fed-146">Windows 管理アプリケーションがインストールされているデバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="20fed-146">Name of the device on which Windows management app is installed.</span></span>|
|<span data-ttu-id="20fed-147">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="20fed-147">deviceOSVersion</span></span>|<span data-ttu-id="20fed-148">String</span><span class="sxs-lookup"><span data-stu-id="20fed-148">String</span></span>|<span data-ttu-id="20fed-149">Windows 管理アプリケーションがインストールされているデバイスの 10 の Windows OS のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="20fed-149">Windows 10 OS version of the device on which Windows management app is installed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="20fed-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="20fed-150">Relationships</span></span>
<span data-ttu-id="20fed-151">なし</span><span class="sxs-lookup"><span data-stu-id="20fed-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="20fed-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20fed-152">JSON Representation</span></span>
<span data-ttu-id="20fed-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20fed-153">Here is a JSON representation of the resource.</span></span>
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





