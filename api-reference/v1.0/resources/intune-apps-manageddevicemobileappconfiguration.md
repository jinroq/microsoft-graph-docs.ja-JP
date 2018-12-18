---
title: managedDeviceMobileAppConfiguration リソースの種類
description: 登録済みデバイスのモバイル アプリ構成用の抽象クラスです。
author: tfitzmac
ms.openlocfilehash: c51db6ddad8b23957da9ed9b8d132c416e52f073
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360026"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="085ed-103">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="085ed-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="085ed-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="085ed-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="085ed-105">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="085ed-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="085ed-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="085ed-106">Methods</span></span>
|<span data-ttu-id="085ed-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="085ed-107">Method</span></span>|<span data-ttu-id="085ed-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="085ed-108">Return Type</span></span>|<span data-ttu-id="085ed-109">説明</span><span class="sxs-lookup"><span data-stu-id="085ed-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="085ed-110">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="085ed-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="085ed-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="085ed-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="085ed-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="085ed-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="085ed-113">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="085ed-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="085ed-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="085ed-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="085ed-115">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="085ed-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="085ed-116">assign action</span><span class="sxs-lookup"><span data-stu-id="085ed-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="085ed-117">なし</span><span class="sxs-lookup"><span data-stu-id="085ed-117">None</span></span>|<span data-ttu-id="085ed-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="085ed-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="085ed-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="085ed-119">Properties</span></span>
|<span data-ttu-id="085ed-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="085ed-120">Property</span></span>|<span data-ttu-id="085ed-121">種類</span><span class="sxs-lookup"><span data-stu-id="085ed-121">Type</span></span>|<span data-ttu-id="085ed-122">説明</span><span class="sxs-lookup"><span data-stu-id="085ed-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="085ed-123">ID</span><span class="sxs-lookup"><span data-stu-id="085ed-123">id</span></span>|<span data-ttu-id="085ed-124">String</span><span class="sxs-lookup"><span data-stu-id="085ed-124">String</span></span>|<span data-ttu-id="085ed-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="085ed-125">Key of the entity.</span></span>|
|<span data-ttu-id="085ed-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="085ed-126">targetedMobileApps</span></span>|<span data-ttu-id="085ed-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="085ed-127">String collection</span></span>|<span data-ttu-id="085ed-128">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="085ed-128">the associated app.</span></span>|
|<span data-ttu-id="085ed-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="085ed-129">createdDateTime</span></span>|<span data-ttu-id="085ed-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="085ed-130">DateTimeOffset</span></span>|<span data-ttu-id="085ed-131">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="085ed-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="085ed-132">説明</span><span class="sxs-lookup"><span data-stu-id="085ed-132">description</span></span>|<span data-ttu-id="085ed-133">String</span><span class="sxs-lookup"><span data-stu-id="085ed-133">String</span></span>|<span data-ttu-id="085ed-134">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="085ed-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="085ed-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="085ed-135">lastModifiedDateTime</span></span>|<span data-ttu-id="085ed-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="085ed-136">DateTimeOffset</span></span>|<span data-ttu-id="085ed-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="085ed-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="085ed-138">displayName</span><span class="sxs-lookup"><span data-stu-id="085ed-138">displayName</span></span>|<span data-ttu-id="085ed-139">String</span><span class="sxs-lookup"><span data-stu-id="085ed-139">String</span></span>|<span data-ttu-id="085ed-140">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="085ed-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="085ed-141">version</span><span class="sxs-lookup"><span data-stu-id="085ed-141">version</span></span>|<span data-ttu-id="085ed-142">Int32</span><span class="sxs-lookup"><span data-stu-id="085ed-142">Int32</span></span>|<span data-ttu-id="085ed-143">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="085ed-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="085ed-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="085ed-144">Relationships</span></span>
|<span data-ttu-id="085ed-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="085ed-145">Relationship</span></span>|<span data-ttu-id="085ed-146">型</span><span class="sxs-lookup"><span data-stu-id="085ed-146">Type</span></span>|<span data-ttu-id="085ed-147">説明</span><span class="sxs-lookup"><span data-stu-id="085ed-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="085ed-148">assignments</span><span class="sxs-lookup"><span data-stu-id="085ed-148">assignments</span></span>|<span data-ttu-id="085ed-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="085ed-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="085ed-150">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="085ed-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="085ed-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="085ed-151">deviceStatuses</span></span>|<span data-ttu-id="085ed-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="085ed-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="085ed-153">ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="085ed-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="085ed-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="085ed-154">userStatuses</span></span>|<span data-ttu-id="085ed-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="085ed-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="085ed-156">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="085ed-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="085ed-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="085ed-157">deviceStatusSummary</span></span>|[<span data-ttu-id="085ed-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="085ed-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="085ed-159">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="085ed-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="085ed-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="085ed-160">userStatusSummary</span></span>|[<span data-ttu-id="085ed-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="085ed-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="085ed-162">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="085ed-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="085ed-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="085ed-163">JSON Representation</span></span>
<span data-ttu-id="085ed-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="085ed-164">Here is a JSON representation of the resource.</span></span>
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



