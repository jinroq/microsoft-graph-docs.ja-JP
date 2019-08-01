---
title: managedDeviceMobileAppConfiguration リソースの種類
description: 登録済みデバイスのモバイル アプリ構成用の抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a833936d24594159708d7dfe3fc8a451d0893e98
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029051"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="3f4a6-103">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f4a6-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="3f4a6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f4a6-105">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-105">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="3f4a6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f4a6-106">Methods</span></span>
|<span data-ttu-id="3f4a6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f4a6-107">Method</span></span>|<span data-ttu-id="3f4a6-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3f4a6-108">Return Type</span></span>|<span data-ttu-id="3f4a6-109">説明</span><span class="sxs-lookup"><span data-stu-id="3f4a6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f4a6-110">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="3f4a6-110">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="3f4a6-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3f4a6-111">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="3f4a6-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-112">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="3f4a6-113">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="3f4a6-113">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="3f4a6-114">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="3f4a6-114">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="3f4a6-115">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-115">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="3f4a6-116">assign アクション</span><span class="sxs-lookup"><span data-stu-id="3f4a6-116">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="3f4a6-117">なし</span><span class="sxs-lookup"><span data-stu-id="3f4a6-117">None</span></span>|<span data-ttu-id="3f4a6-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3f4a6-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3f4a6-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f4a6-119">Properties</span></span>
|<span data-ttu-id="3f4a6-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f4a6-120">Property</span></span>|<span data-ttu-id="3f4a6-121">型</span><span class="sxs-lookup"><span data-stu-id="3f4a6-121">Type</span></span>|<span data-ttu-id="3f4a6-122">説明</span><span class="sxs-lookup"><span data-stu-id="3f4a6-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4a6-123">id</span><span class="sxs-lookup"><span data-stu-id="3f4a6-123">id</span></span>|<span data-ttu-id="3f4a6-124">文字列</span><span class="sxs-lookup"><span data-stu-id="3f4a6-124">String</span></span>|<span data-ttu-id="3f4a6-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-125">Key of the entity.</span></span>|
|<span data-ttu-id="3f4a6-126">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="3f4a6-126">targetedMobileApps</span></span>|<span data-ttu-id="3f4a6-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3f4a6-127">String collection</span></span>|<span data-ttu-id="3f4a6-128">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-128">the associated app.</span></span>|
|<span data-ttu-id="3f4a6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f4a6-129">createdDateTime</span></span>|<span data-ttu-id="3f4a6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f4a6-130">DateTimeOffset</span></span>|<span data-ttu-id="3f4a6-131">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-131">DateTime the object was created.</span></span>|
|<span data-ttu-id="3f4a6-132">description</span><span class="sxs-lookup"><span data-stu-id="3f4a6-132">description</span></span>|<span data-ttu-id="3f4a6-133">String</span><span class="sxs-lookup"><span data-stu-id="3f4a6-133">String</span></span>|<span data-ttu-id="3f4a6-134">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-134">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="3f4a6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f4a6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3f4a6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f4a6-136">DateTimeOffset</span></span>|<span data-ttu-id="3f4a6-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="3f4a6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3f4a6-138">displayName</span></span>|<span data-ttu-id="3f4a6-139">String</span><span class="sxs-lookup"><span data-stu-id="3f4a6-139">String</span></span>|<span data-ttu-id="3f4a6-140">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-140">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="3f4a6-141">version</span><span class="sxs-lookup"><span data-stu-id="3f4a6-141">version</span></span>|<span data-ttu-id="3f4a6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="3f4a6-142">Int32</span></span>|<span data-ttu-id="3f4a6-143">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-143">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f4a6-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f4a6-144">Relationships</span></span>
|<span data-ttu-id="3f4a6-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f4a6-145">Relationship</span></span>|<span data-ttu-id="3f4a6-146">型</span><span class="sxs-lookup"><span data-stu-id="3f4a6-146">Type</span></span>|<span data-ttu-id="3f4a6-147">説明</span><span class="sxs-lookup"><span data-stu-id="3f4a6-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f4a6-148">assignments</span><span class="sxs-lookup"><span data-stu-id="3f4a6-148">assignments</span></span>|<span data-ttu-id="3f4a6-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3f4a6-149">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="3f4a6-150">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-150">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="3f4a6-151">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="3f4a6-151">deviceStatuses</span></span>|<span data-ttu-id="3f4a6-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3f4a6-152">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="3f4a6-153">ManagedDeviceMobileAppConfigurationDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-153">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="3f4a6-154">userStatuses</span><span class="sxs-lookup"><span data-stu-id="3f4a6-154">userStatuses</span></span>|<span data-ttu-id="3f4a6-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3f4a6-155">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="3f4a6-156">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-156">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="3f4a6-157">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="3f4a6-157">deviceStatusSummary</span></span>|[<span data-ttu-id="3f4a6-158">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="3f4a6-158">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="3f4a6-159">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-159">App configuration device status summary.</span></span>|
|<span data-ttu-id="3f4a6-160">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="3f4a6-160">userStatusSummary</span></span>|[<span data-ttu-id="3f4a6-161">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="3f4a6-161">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="3f4a6-162">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-162">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f4a6-163">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f4a6-163">JSON Representation</span></span>
<span data-ttu-id="3f4a6-164">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f4a6-164">Here is a JSON representation of the resource.</span></span>
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



