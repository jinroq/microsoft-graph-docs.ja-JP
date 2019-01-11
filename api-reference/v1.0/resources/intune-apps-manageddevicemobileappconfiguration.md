---
title: managedDeviceMobileAppConfiguration リソースの種類
description: 登録済みデバイスのモバイル アプリ構成用の抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e2ad71a4927f2b0156d085bad54cf59d45f97c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811649"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="2ff30-103">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ff30-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="2ff30-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ff30-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2ff30-105">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="2ff30-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="2ff30-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ff30-106">Methods</span></span>
|<span data-ttu-id="2ff30-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ff30-107">Method</span></span>|<span data-ttu-id="2ff30-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ff30-108">Return Type</span></span>|<span data-ttu-id="2ff30-109">説明</span><span class="sxs-lookup"><span data-stu-id="2ff30-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ff30-110">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="2ff30-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="2ff30-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ff30-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="2ff30-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2ff30-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2ff30-113">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="2ff30-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="2ff30-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ff30-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="2ff30-115">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ff30-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="2ff30-116">assign action</span><span class="sxs-lookup"><span data-stu-id="2ff30-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="2ff30-117">なし</span><span class="sxs-lookup"><span data-stu-id="2ff30-117">None</span></span>|<span data-ttu-id="2ff30-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2ff30-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2ff30-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ff30-119">Properties</span></span>
|<span data-ttu-id="2ff30-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ff30-120">Property</span></span>|<span data-ttu-id="2ff30-121">種類</span><span class="sxs-lookup"><span data-stu-id="2ff30-121">Type</span></span>|<span data-ttu-id="2ff30-122">説明</span><span class="sxs-lookup"><span data-stu-id="2ff30-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff30-123">ID</span><span class="sxs-lookup"><span data-stu-id="2ff30-123">id</span></span>|<span data-ttu-id="2ff30-124">String</span><span class="sxs-lookup"><span data-stu-id="2ff30-124">String</span></span>|<span data-ttu-id="2ff30-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ff30-125">Key of the entity.</span></span>|
|<span data-ttu-id="2ff30-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="2ff30-126">targetedMobileApps</span></span>|<span data-ttu-id="2ff30-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="2ff30-127">String collection</span></span>|<span data-ttu-id="2ff30-128">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="2ff30-128">the associated app.</span></span>|
|<span data-ttu-id="2ff30-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff30-129">createdDateTime</span></span>|<span data-ttu-id="2ff30-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff30-130">DateTimeOffset</span></span>|<span data-ttu-id="2ff30-131">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2ff30-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="2ff30-132">説明</span><span class="sxs-lookup"><span data-stu-id="2ff30-132">description</span></span>|<span data-ttu-id="2ff30-133">String</span><span class="sxs-lookup"><span data-stu-id="2ff30-133">String</span></span>|<span data-ttu-id="2ff30-134">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="2ff30-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="2ff30-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ff30-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2ff30-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff30-136">DateTimeOffset</span></span>|<span data-ttu-id="2ff30-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2ff30-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="2ff30-138">displayName</span><span class="sxs-lookup"><span data-stu-id="2ff30-138">displayName</span></span>|<span data-ttu-id="2ff30-139">String</span><span class="sxs-lookup"><span data-stu-id="2ff30-139">String</span></span>|<span data-ttu-id="2ff30-140">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="2ff30-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="2ff30-141">version</span><span class="sxs-lookup"><span data-stu-id="2ff30-141">version</span></span>|<span data-ttu-id="2ff30-142">Int32</span><span class="sxs-lookup"><span data-stu-id="2ff30-142">Int32</span></span>|<span data-ttu-id="2ff30-143">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ff30-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ff30-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ff30-144">Relationships</span></span>
|<span data-ttu-id="2ff30-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ff30-145">Relationship</span></span>|<span data-ttu-id="2ff30-146">型</span><span class="sxs-lookup"><span data-stu-id="2ff30-146">Type</span></span>|<span data-ttu-id="2ff30-147">説明</span><span class="sxs-lookup"><span data-stu-id="2ff30-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff30-148">assignments</span><span class="sxs-lookup"><span data-stu-id="2ff30-148">assignments</span></span>|<span data-ttu-id="2ff30-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ff30-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2ff30-150">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="2ff30-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="2ff30-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="2ff30-151">deviceStatuses</span></span>|<span data-ttu-id="2ff30-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2ff30-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="2ff30-153">ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="2ff30-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="2ff30-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="2ff30-154">userStatuses</span></span>|<span data-ttu-id="2ff30-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ff30-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="2ff30-156">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="2ff30-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="2ff30-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="2ff30-157">deviceStatusSummary</span></span>|[<span data-ttu-id="2ff30-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="2ff30-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="2ff30-159">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="2ff30-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="2ff30-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="2ff30-160">userStatusSummary</span></span>|[<span data-ttu-id="2ff30-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="2ff30-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="2ff30-162">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="2ff30-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ff30-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ff30-163">JSON Representation</span></span>
<span data-ttu-id="2ff30-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ff30-164">Here is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```



