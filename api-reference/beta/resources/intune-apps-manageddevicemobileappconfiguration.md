---
title: managedDeviceMobileAppConfiguration リソースの種類
description: 登録済みデバイスのモバイル アプリ構成用の抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f9a642f00e9dce09628083a8278e6010a220bee2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918988"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="35eb3-103">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35eb3-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="35eb3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="35eb3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="35eb3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35eb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35eb3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35eb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35eb3-107">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="35eb3-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="35eb3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="35eb3-108">Methods</span></span>
|<span data-ttu-id="35eb3-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="35eb3-109">Method</span></span>|<span data-ttu-id="35eb3-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="35eb3-110">Return Type</span></span>|<span data-ttu-id="35eb3-111">説明</span><span class="sxs-lookup"><span data-stu-id="35eb3-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="35eb3-112">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="35eb3-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="35eb3-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35eb3-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="35eb3-114">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="35eb3-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="35eb3-115">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="35eb3-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="35eb3-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="35eb3-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="35eb3-117">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="35eb3-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="35eb3-118">assign action</span><span class="sxs-lookup"><span data-stu-id="35eb3-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="35eb3-119">なし</span><span class="sxs-lookup"><span data-stu-id="35eb3-119">None</span></span>|<span data-ttu-id="35eb3-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="35eb3-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="35eb3-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35eb3-121">Properties</span></span>
|<span data-ttu-id="35eb3-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35eb3-122">Property</span></span>|<span data-ttu-id="35eb3-123">型</span><span class="sxs-lookup"><span data-stu-id="35eb3-123">Type</span></span>|<span data-ttu-id="35eb3-124">説明</span><span class="sxs-lookup"><span data-stu-id="35eb3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35eb3-125">ID</span><span class="sxs-lookup"><span data-stu-id="35eb3-125">id</span></span>|<span data-ttu-id="35eb3-126">String</span><span class="sxs-lookup"><span data-stu-id="35eb3-126">String</span></span>|<span data-ttu-id="35eb3-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="35eb3-127">Key of the entity.</span></span>|
|<span data-ttu-id="35eb3-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="35eb3-128">targetedMobileApps</span></span>|<span data-ttu-id="35eb3-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="35eb3-129">String collection</span></span>|<span data-ttu-id="35eb3-130">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="35eb3-130">the associated app.</span></span>|
|<span data-ttu-id="35eb3-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="35eb3-131">roleScopeTagIds</span></span>|<span data-ttu-id="35eb3-132">String コレクション</span><span class="sxs-lookup"><span data-stu-id="35eb3-132">String collection</span></span>|<span data-ttu-id="35eb3-133">このアプリケーションの構成エンティティのスコープのタグの一覧です。</span><span class="sxs-lookup"><span data-stu-id="35eb3-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="35eb3-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="35eb3-134">createdDateTime</span></span>|<span data-ttu-id="35eb3-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35eb3-135">DateTimeOffset</span></span>|<span data-ttu-id="35eb3-136">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="35eb3-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="35eb3-137">説明</span><span class="sxs-lookup"><span data-stu-id="35eb3-137">description</span></span>|<span data-ttu-id="35eb3-138">String</span><span class="sxs-lookup"><span data-stu-id="35eb3-138">String</span></span>|<span data-ttu-id="35eb3-139">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="35eb3-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="35eb3-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="35eb3-140">lastModifiedDateTime</span></span>|<span data-ttu-id="35eb3-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="35eb3-141">DateTimeOffset</span></span>|<span data-ttu-id="35eb3-142">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="35eb3-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="35eb3-143">displayName</span><span class="sxs-lookup"><span data-stu-id="35eb3-143">displayName</span></span>|<span data-ttu-id="35eb3-144">String</span><span class="sxs-lookup"><span data-stu-id="35eb3-144">String</span></span>|<span data-ttu-id="35eb3-145">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="35eb3-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="35eb3-146">version</span><span class="sxs-lookup"><span data-stu-id="35eb3-146">version</span></span>|<span data-ttu-id="35eb3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="35eb3-147">Int32</span></span>|<span data-ttu-id="35eb3-148">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="35eb3-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35eb3-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35eb3-149">Relationships</span></span>
|<span data-ttu-id="35eb3-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="35eb3-150">Relationship</span></span>|<span data-ttu-id="35eb3-151">型</span><span class="sxs-lookup"><span data-stu-id="35eb3-151">Type</span></span>|<span data-ttu-id="35eb3-152">説明</span><span class="sxs-lookup"><span data-stu-id="35eb3-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35eb3-153">assignments</span><span class="sxs-lookup"><span data-stu-id="35eb3-153">assignments</span></span>|<span data-ttu-id="35eb3-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35eb3-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="35eb3-155">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="35eb3-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="35eb3-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="35eb3-156">deviceStatuses</span></span>|<span data-ttu-id="35eb3-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="35eb3-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="35eb3-158">ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="35eb3-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="35eb3-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="35eb3-159">userStatuses</span></span>|<span data-ttu-id="35eb3-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="35eb3-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="35eb3-161">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="35eb3-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="35eb3-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="35eb3-162">deviceStatusSummary</span></span>|[<span data-ttu-id="35eb3-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="35eb3-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="35eb3-164">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="35eb3-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="35eb3-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="35eb3-165">userStatusSummary</span></span>|[<span data-ttu-id="35eb3-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="35eb3-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="35eb3-167">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="35eb3-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35eb3-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35eb3-168">JSON Representation</span></span>
<span data-ttu-id="35eb3-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35eb3-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```





