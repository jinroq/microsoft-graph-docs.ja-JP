---
title: managedDeviceMobileAppConfiguration リソースの種類
description: 登録済みデバイスのモバイル アプリ構成用の抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4646ebc07865cadda7005e25b4b30a2547a41f8b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552186"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="b3696-103">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3696-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="b3696-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3696-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3696-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b3696-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3696-106">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="b3696-106">An abstract class for Mobile app configuration for enrolled devices.</span></span>

## <a name="methods"></a><span data-ttu-id="b3696-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3696-107">Methods</span></span>
|<span data-ttu-id="b3696-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3696-108">Method</span></span>|<span data-ttu-id="b3696-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b3696-109">Return Type</span></span>|<span data-ttu-id="b3696-110">説明</span><span class="sxs-lookup"><span data-stu-id="b3696-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b3696-111">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="b3696-111">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="b3696-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b3696-112">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="b3696-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b3696-113">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b3696-114">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="b3696-114">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="b3696-115">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3696-115">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="b3696-116">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b3696-116">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="b3696-117">assign アクション</span><span class="sxs-lookup"><span data-stu-id="b3696-117">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="b3696-118">なし</span><span class="sxs-lookup"><span data-stu-id="b3696-118">None</span></span>|<span data-ttu-id="b3696-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="b3696-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="b3696-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3696-120">Properties</span></span>
|<span data-ttu-id="b3696-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3696-121">Property</span></span>|<span data-ttu-id="b3696-122">型</span><span class="sxs-lookup"><span data-stu-id="b3696-122">Type</span></span>|<span data-ttu-id="b3696-123">説明</span><span class="sxs-lookup"><span data-stu-id="b3696-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3696-124">id</span><span class="sxs-lookup"><span data-stu-id="b3696-124">id</span></span>|<span data-ttu-id="b3696-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b3696-125">String</span></span>|<span data-ttu-id="b3696-126">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b3696-126">Key of the entity.</span></span>|
|<span data-ttu-id="b3696-127">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="b3696-127">targetedMobileApps</span></span>|<span data-ttu-id="b3696-128">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b3696-128">String collection</span></span>|<span data-ttu-id="b3696-129">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="b3696-129">the associated app.</span></span>|
|<span data-ttu-id="b3696-130">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3696-130">roleScopeTagIds</span></span>|<span data-ttu-id="b3696-131">String collection</span><span class="sxs-lookup"><span data-stu-id="b3696-131">String collection</span></span>|<span data-ttu-id="b3696-132">このアプリ構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b3696-132">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="b3696-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3696-133">createdDateTime</span></span>|<span data-ttu-id="b3696-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3696-134">DateTimeOffset</span></span>|<span data-ttu-id="b3696-135">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b3696-135">DateTime the object was created.</span></span>|
|<span data-ttu-id="b3696-136">description</span><span class="sxs-lookup"><span data-stu-id="b3696-136">description</span></span>|<span data-ttu-id="b3696-137">String</span><span class="sxs-lookup"><span data-stu-id="b3696-137">String</span></span>|<span data-ttu-id="b3696-138">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="b3696-138">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="b3696-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3696-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b3696-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3696-140">DateTimeOffset</span></span>|<span data-ttu-id="b3696-141">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b3696-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b3696-142">displayName</span><span class="sxs-lookup"><span data-stu-id="b3696-142">displayName</span></span>|<span data-ttu-id="b3696-143">String</span><span class="sxs-lookup"><span data-stu-id="b3696-143">String</span></span>|<span data-ttu-id="b3696-144">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="b3696-144">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="b3696-145">version</span><span class="sxs-lookup"><span data-stu-id="b3696-145">version</span></span>|<span data-ttu-id="b3696-146">Int32</span><span class="sxs-lookup"><span data-stu-id="b3696-146">Int32</span></span>|<span data-ttu-id="b3696-147">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b3696-147">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3696-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3696-148">Relationships</span></span>
|<span data-ttu-id="b3696-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3696-149">Relationship</span></span>|<span data-ttu-id="b3696-150">型</span><span class="sxs-lookup"><span data-stu-id="b3696-150">Type</span></span>|<span data-ttu-id="b3696-151">説明</span><span class="sxs-lookup"><span data-stu-id="b3696-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3696-152">assignments</span><span class="sxs-lookup"><span data-stu-id="b3696-152">assignments</span></span>|<span data-ttu-id="b3696-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b3696-153">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="b3696-154">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="b3696-154">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="b3696-155">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b3696-155">deviceStatuses</span></span>|<span data-ttu-id="b3696-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b3696-156">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b3696-157">ManagedDeviceMobileAppConfigurationDeviceStatus のリスト。</span><span class="sxs-lookup"><span data-stu-id="b3696-157">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="b3696-158">userStatuses</span><span class="sxs-lookup"><span data-stu-id="b3696-158">userStatuses</span></span>|<span data-ttu-id="b3696-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b3696-159">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="b3696-160">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="b3696-160">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="b3696-161">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b3696-161">deviceStatusSummary</span></span>|[<span data-ttu-id="b3696-162">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="b3696-162">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="b3696-163">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="b3696-163">App configuration device status summary.</span></span>|
|<span data-ttu-id="b3696-164">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="b3696-164">userStatusSummary</span></span>|[<span data-ttu-id="b3696-165">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="b3696-165">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="b3696-166">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="b3696-166">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3696-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3696-167">JSON Representation</span></span>
<span data-ttu-id="b3696-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3696-168">Here is a JSON representation of the resource.</span></span>
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





