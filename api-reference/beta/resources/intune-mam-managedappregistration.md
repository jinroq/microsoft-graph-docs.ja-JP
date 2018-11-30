---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
ms.openlocfilehash: bf05e7180f27be9c813f8fbb05346893fa6db172
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069449"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="46450-103">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="46450-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="46450-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46450-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46450-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46450-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46450-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="46450-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="46450-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="46450-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="46450-108">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="46450-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="46450-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="46450-109">Methods</span></span>
|<span data-ttu-id="46450-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="46450-110">Method</span></span>|<span data-ttu-id="46450-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="46450-111">Return Type</span></span>|<span data-ttu-id="46450-112">説明</span><span class="sxs-lookup"><span data-stu-id="46450-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="46450-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="46450-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="46450-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46450-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="46450-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="46450-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="46450-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="46450-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="46450-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="46450-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="46450-118">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="46450-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="46450-119">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="46450-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="46450-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="46450-120">String collection</span></span>|<span data-ttu-id="46450-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="46450-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="46450-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46450-122">Properties</span></span>
|<span data-ttu-id="46450-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46450-123">Property</span></span>|<span data-ttu-id="46450-124">型</span><span class="sxs-lookup"><span data-stu-id="46450-124">Type</span></span>|<span data-ttu-id="46450-125">説明</span><span class="sxs-lookup"><span data-stu-id="46450-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46450-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="46450-126">createdDateTime</span></span>|<span data-ttu-id="46450-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46450-127">DateTimeOffset</span></span>|<span data-ttu-id="46450-128">作成日時</span><span class="sxs-lookup"><span data-stu-id="46450-128">Date and time of creation</span></span>|
|<span data-ttu-id="46450-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="46450-129">lastSyncDateTime</span></span>|<span data-ttu-id="46450-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46450-130">DateTimeOffset</span></span>|<span data-ttu-id="46450-131">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="46450-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="46450-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="46450-132">applicationVersion</span></span>|<span data-ttu-id="46450-133">String</span><span class="sxs-lookup"><span data-stu-id="46450-133">String</span></span>|<span data-ttu-id="46450-134">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="46450-134">App version</span></span>|
|<span data-ttu-id="46450-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="46450-135">managementSdkVersion</span></span>|<span data-ttu-id="46450-136">String</span><span class="sxs-lookup"><span data-stu-id="46450-136">String</span></span>|<span data-ttu-id="46450-137">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="46450-137">App management SDK version</span></span>|
|<span data-ttu-id="46450-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="46450-138">platformVersion</span></span>|<span data-ttu-id="46450-139">String</span><span class="sxs-lookup"><span data-stu-id="46450-139">String</span></span>|<span data-ttu-id="46450-140">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="46450-140">Operating System version</span></span>|
|<span data-ttu-id="46450-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="46450-141">deviceType</span></span>|<span data-ttu-id="46450-142">String</span><span class="sxs-lookup"><span data-stu-id="46450-142">String</span></span>|<span data-ttu-id="46450-143">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="46450-143">Host device type</span></span>|
|<span data-ttu-id="46450-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="46450-144">deviceTag</span></span>|<span data-ttu-id="46450-145">String</span><span class="sxs-lookup"><span data-stu-id="46450-145">String</span></span>|<span data-ttu-id="46450-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="46450-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="46450-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="46450-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="46450-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="46450-148">deviceName</span></span>|<span data-ttu-id="46450-149">String</span><span class="sxs-lookup"><span data-stu-id="46450-149">String</span></span>|<span data-ttu-id="46450-150">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="46450-150">Host device name</span></span>|
|<span data-ttu-id="46450-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="46450-151">managedDeviceId</span></span>|<span data-ttu-id="46450-152">String</span><span class="sxs-lookup"><span data-stu-id="46450-152">String</span></span>|<span data-ttu-id="46450-153">ホスト ・ デバイスの管理デバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="46450-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="46450-154">ホスト ・ デバイスが管理されている場合にも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="46450-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="46450-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="46450-155">azureADDeviceId</span></span>|<span data-ttu-id="46450-156">String</span><span class="sxs-lookup"><span data-stu-id="46450-156">String</span></span>|<span data-ttu-id="46450-157">ホスト ・ デバイスの Azure Active Directory のデバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="46450-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="46450-158">ホスト ・ デバイスは、Azure Active Directory が登録されている場合でも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="46450-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="46450-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="46450-159">deviceModel</span></span>|<span data-ttu-id="46450-160">String</span><span class="sxs-lookup"><span data-stu-id="46450-160">String</span></span>|<span data-ttu-id="46450-161">現在のアプリケーションの登録用のデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="46450-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="46450-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="46450-162">deviceManufacturer</span></span>|<span data-ttu-id="46450-163">String</span><span class="sxs-lookup"><span data-stu-id="46450-163">String</span></span>|<span data-ttu-id="46450-164">現在のアプリケーションの登録のためのデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="46450-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="46450-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="46450-165">flaggedReasons</span></span>|<span data-ttu-id="46450-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="46450-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="46450-167">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="46450-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="46450-168">例:</span><span class="sxs-lookup"><span data-stu-id="46450-168">E.g.</span></span> <span data-ttu-id="46450-169">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="46450-169">app running on rooted device</span></span>|
|<span data-ttu-id="46450-170">userId</span><span class="sxs-lookup"><span data-stu-id="46450-170">userId</span></span>|<span data-ttu-id="46450-171">String</span><span class="sxs-lookup"><span data-stu-id="46450-171">String</span></span>|<span data-ttu-id="46450-172">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="46450-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="46450-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="46450-173">appIdentifier</span></span>|[<span data-ttu-id="46450-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="46450-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="46450-175">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="46450-175">The app package Identifier</span></span>|
|<span data-ttu-id="46450-176">id</span><span class="sxs-lookup"><span data-stu-id="46450-176">id</span></span>|<span data-ttu-id="46450-177">String</span><span class="sxs-lookup"><span data-stu-id="46450-177">String</span></span>|<span data-ttu-id="46450-178">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="46450-178">Key of the entity.</span></span>|
|<span data-ttu-id="46450-179">version</span><span class="sxs-lookup"><span data-stu-id="46450-179">version</span></span>|<span data-ttu-id="46450-180">String</span><span class="sxs-lookup"><span data-stu-id="46450-180">String</span></span>|<span data-ttu-id="46450-181">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="46450-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="46450-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46450-182">Relationships</span></span>
|<span data-ttu-id="46450-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="46450-183">Relationship</span></span>|<span data-ttu-id="46450-184">型</span><span class="sxs-lookup"><span data-stu-id="46450-184">Type</span></span>|<span data-ttu-id="46450-185">説明</span><span class="sxs-lookup"><span data-stu-id="46450-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46450-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="46450-186">appliedPolicies</span></span>|<span data-ttu-id="46450-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46450-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="46450-188">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="46450-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="46450-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="46450-189">intendedPolicies</span></span>|<span data-ttu-id="46450-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46450-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="46450-191">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="46450-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="46450-192">operations</span><span class="sxs-lookup"><span data-stu-id="46450-192">operations</span></span>|<span data-ttu-id="46450-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="46450-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="46450-194">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="46450-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="46450-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="46450-195">JSON Representation</span></span>
<span data-ttu-id="46450-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="46450-196">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppRegistration",
  "createdDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "applicationVersion": "String",
  "managementSdkVersion": "String",
  "platformVersion": "String",
  "deviceType": "String",
  "deviceTag": "String",
  "deviceName": "String",
  "managedDeviceId": "String",
  "azureADDeviceId": "String",
  "deviceModel": "String",
  "deviceManufacturer": "String",
  "flaggedReasons": [
    "String"
  ],
  "userId": "String",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```





