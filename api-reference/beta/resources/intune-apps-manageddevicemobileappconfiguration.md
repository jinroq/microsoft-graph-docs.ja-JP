---
title: managedDeviceMobileAppConfiguration リソースの種類
description: 登録済みデバイスのモバイル アプリ構成用の抽象クラスです。
author: tfitzmac
ms.openlocfilehash: a533d5d7c15a32d811a7fd23f9ab39b89db9b7da
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352039"
---
# <a name="manageddevicemobileappconfiguration-resource-type"></a><span data-ttu-id="5e8f0-103">managedDeviceMobileAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e8f0-103">managedDeviceMobileAppConfiguration resource type</span></span>

> <span data-ttu-id="5e8f0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5e8f0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5e8f0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e8f0-107">登録済みデバイスのモバイル アプリ構成用の抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-107">An abstract class for Mobile app configuration for enrolled devices.</span></span>
## <a name="methods"></a><span data-ttu-id="5e8f0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5e8f0-108">Methods</span></span>
|<span data-ttu-id="5e8f0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5e8f0-109">Method</span></span>|<span data-ttu-id="5e8f0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5e8f0-110">Return Type</span></span>|<span data-ttu-id="5e8f0-111">説明</span><span class="sxs-lookup"><span data-stu-id="5e8f0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5e8f0-112">managedDeviceMobileAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="5e8f0-112">List managedDeviceMobileAppConfigurations</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-list.md)|<span data-ttu-id="5e8f0-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5e8f0-113">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) collection</span></span>|<span data-ttu-id="5e8f0-114">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-114">List properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="5e8f0-115">managedDeviceMobileAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="5e8f0-115">Get managedDeviceMobileAppConfiguration</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-get.md)|[<span data-ttu-id="5e8f0-116">managedDeviceMobileAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="5e8f0-116">managedDeviceMobileAppConfiguration</span></span>](../resources/intune-apps-manageddevicemobileappconfiguration.md)|<span data-ttu-id="5e8f0-117">[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-117">Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) object.</span></span>|
|[<span data-ttu-id="5e8f0-118">assign action</span><span class="sxs-lookup"><span data-stu-id="5e8f0-118">assign action</span></span>](../api/intune-apps-manageddevicemobileappconfiguration-assign.md)|<span data-ttu-id="5e8f0-119">なし</span><span class="sxs-lookup"><span data-stu-id="5e8f0-119">None</span></span>|<span data-ttu-id="5e8f0-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5e8f0-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5e8f0-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e8f0-121">Properties</span></span>
|<span data-ttu-id="5e8f0-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e8f0-122">Property</span></span>|<span data-ttu-id="5e8f0-123">種類</span><span class="sxs-lookup"><span data-stu-id="5e8f0-123">Type</span></span>|<span data-ttu-id="5e8f0-124">説明</span><span class="sxs-lookup"><span data-stu-id="5e8f0-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8f0-125">ID</span><span class="sxs-lookup"><span data-stu-id="5e8f0-125">id</span></span>|<span data-ttu-id="5e8f0-126">String</span><span class="sxs-lookup"><span data-stu-id="5e8f0-126">String</span></span>|<span data-ttu-id="5e8f0-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-127">Key of the entity.</span></span>|
|<span data-ttu-id="5e8f0-128">targetedMobileApps</span><span class="sxs-lookup"><span data-stu-id="5e8f0-128">targetedMobileApps</span></span>|<span data-ttu-id="5e8f0-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5e8f0-129">String collection</span></span>|<span data-ttu-id="5e8f0-130">関連するアプリです。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-130">the associated app.</span></span>|
|<span data-ttu-id="5e8f0-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5e8f0-131">roleScopeTagIds</span></span>|<span data-ttu-id="5e8f0-132">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5e8f0-132">String collection</span></span>|<span data-ttu-id="5e8f0-133">このアプリケーションの構成エンティティのスコープのタグの一覧です。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-133">List of Scope Tags for this App configuration entity.</span></span>|
|<span data-ttu-id="5e8f0-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8f0-134">createdDateTime</span></span>|<span data-ttu-id="5e8f0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e8f0-135">DateTimeOffset</span></span>|<span data-ttu-id="5e8f0-136">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-136">DateTime the object was created.</span></span>|
|<span data-ttu-id="5e8f0-137">説明</span><span class="sxs-lookup"><span data-stu-id="5e8f0-137">description</span></span>|<span data-ttu-id="5e8f0-138">String</span><span class="sxs-lookup"><span data-stu-id="5e8f0-138">String</span></span>|<span data-ttu-id="5e8f0-139">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-139">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="5e8f0-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5e8f0-140">lastModifiedDateTime</span></span>|<span data-ttu-id="5e8f0-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e8f0-141">DateTimeOffset</span></span>|<span data-ttu-id="5e8f0-142">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5e8f0-143">displayName</span><span class="sxs-lookup"><span data-stu-id="5e8f0-143">displayName</span></span>|<span data-ttu-id="5e8f0-144">String</span><span class="sxs-lookup"><span data-stu-id="5e8f0-144">String</span></span>|<span data-ttu-id="5e8f0-145">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-145">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5e8f0-146">version</span><span class="sxs-lookup"><span data-stu-id="5e8f0-146">version</span></span>|<span data-ttu-id="5e8f0-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5e8f0-147">Int32</span></span>|<span data-ttu-id="5e8f0-148">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-148">Version of the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e8f0-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5e8f0-149">Relationships</span></span>
|<span data-ttu-id="5e8f0-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5e8f0-150">Relationship</span></span>|<span data-ttu-id="5e8f0-151">型</span><span class="sxs-lookup"><span data-stu-id="5e8f0-151">Type</span></span>|<span data-ttu-id="5e8f0-152">説明</span><span class="sxs-lookup"><span data-stu-id="5e8f0-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e8f0-153">assignments</span><span class="sxs-lookup"><span data-stu-id="5e8f0-153">assignments</span></span>|<span data-ttu-id="5e8f0-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5e8f0-154">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) collection</span></span>|<span data-ttu-id="5e8f0-155">アプリ構成のグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-155">The list of group assignemenets for app configration.</span></span>|
|<span data-ttu-id="5e8f0-156">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="5e8f0-156">deviceStatuses</span></span>|<span data-ttu-id="5e8f0-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5e8f0-157">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="5e8f0-158">ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-158">List of ManagedDeviceMobileAppConfigurationDeviceStatus.</span></span>|
|<span data-ttu-id="5e8f0-159">userStatuses</span><span class="sxs-lookup"><span data-stu-id="5e8f0-159">userStatuses</span></span>|<span data-ttu-id="5e8f0-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5e8f0-160">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="5e8f0-161">ManagedDeviceMobileAppConfigurationUserStatus のリストです。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-161">List of ManagedDeviceMobileAppConfigurationUserStatus.</span></span>|
|<span data-ttu-id="5e8f0-162">deviceStatusSummary</span><span class="sxs-lookup"><span data-stu-id="5e8f0-162">deviceStatusSummary</span></span>|[<span data-ttu-id="5e8f0-163">managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="5e8f0-163">managedDeviceMobileAppConfigurationDeviceSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|<span data-ttu-id="5e8f0-164">アプリ構成のデバイス状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-164">App configuration device status summary.</span></span>|
|<span data-ttu-id="5e8f0-165">userStatusSummary</span><span class="sxs-lookup"><span data-stu-id="5e8f0-165">userStatusSummary</span></span>|[<span data-ttu-id="5e8f0-166">managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="5e8f0-166">managedDeviceMobileAppConfigurationUserSummary</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|<span data-ttu-id="5e8f0-167">アプリ構成のユーザー状態の要約です。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-167">App configuration user status summary.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e8f0-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e8f0-168">JSON Representation</span></span>
<span data-ttu-id="5e8f0-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e8f0-169">Here is a JSON representation of the resource.</span></span>
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





