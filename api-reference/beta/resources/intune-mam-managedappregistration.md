---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 959bd294ab1752617cea6a6ea5bbe8f0a3802f0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869721"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="d6578-103">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="d6578-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="d6578-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6578-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6578-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6578-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6578-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6578-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6578-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="d6578-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="d6578-108">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="d6578-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="d6578-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6578-109">Methods</span></span>
|<span data-ttu-id="d6578-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6578-110">Method</span></span>|<span data-ttu-id="d6578-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d6578-111">Return Type</span></span>|<span data-ttu-id="d6578-112">説明</span><span class="sxs-lookup"><span data-stu-id="d6578-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d6578-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d6578-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="d6578-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d6578-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="d6578-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d6578-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="d6578-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d6578-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="d6578-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d6578-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="d6578-118">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d6578-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="d6578-119">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="d6578-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="d6578-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d6578-120">String collection</span></span>|<span data-ttu-id="d6578-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d6578-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d6578-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6578-122">Properties</span></span>
|<span data-ttu-id="d6578-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6578-123">Property</span></span>|<span data-ttu-id="d6578-124">種類</span><span class="sxs-lookup"><span data-stu-id="d6578-124">Type</span></span>|<span data-ttu-id="d6578-125">説明</span><span class="sxs-lookup"><span data-stu-id="d6578-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6578-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6578-126">createdDateTime</span></span>|<span data-ttu-id="d6578-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6578-127">DateTimeOffset</span></span>|<span data-ttu-id="d6578-128">作成日時</span><span class="sxs-lookup"><span data-stu-id="d6578-128">Date and time of creation</span></span>|
|<span data-ttu-id="d6578-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d6578-129">lastSyncDateTime</span></span>|<span data-ttu-id="d6578-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6578-130">DateTimeOffset</span></span>|<span data-ttu-id="d6578-131">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="d6578-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="d6578-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d6578-132">applicationVersion</span></span>|<span data-ttu-id="d6578-133">String</span><span class="sxs-lookup"><span data-stu-id="d6578-133">String</span></span>|<span data-ttu-id="d6578-134">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="d6578-134">App version</span></span>|
|<span data-ttu-id="d6578-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d6578-135">managementSdkVersion</span></span>|<span data-ttu-id="d6578-136">String</span><span class="sxs-lookup"><span data-stu-id="d6578-136">String</span></span>|<span data-ttu-id="d6578-137">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="d6578-137">App management SDK version</span></span>|
|<span data-ttu-id="d6578-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d6578-138">platformVersion</span></span>|<span data-ttu-id="d6578-139">String</span><span class="sxs-lookup"><span data-stu-id="d6578-139">String</span></span>|<span data-ttu-id="d6578-140">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="d6578-140">Operating System version</span></span>|
|<span data-ttu-id="d6578-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="d6578-141">deviceType</span></span>|<span data-ttu-id="d6578-142">String</span><span class="sxs-lookup"><span data-stu-id="d6578-142">String</span></span>|<span data-ttu-id="d6578-143">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="d6578-143">Host device type</span></span>|
|<span data-ttu-id="d6578-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d6578-144">deviceTag</span></span>|<span data-ttu-id="d6578-145">String</span><span class="sxs-lookup"><span data-stu-id="d6578-145">String</span></span>|<span data-ttu-id="d6578-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="d6578-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d6578-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="d6578-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="d6578-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="d6578-148">deviceName</span></span>|<span data-ttu-id="d6578-149">String</span><span class="sxs-lookup"><span data-stu-id="d6578-149">String</span></span>|<span data-ttu-id="d6578-150">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="d6578-150">Host device name</span></span>|
|<span data-ttu-id="d6578-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d6578-151">managedDeviceId</span></span>|<span data-ttu-id="d6578-152">String</span><span class="sxs-lookup"><span data-stu-id="d6578-152">String</span></span>|<span data-ttu-id="d6578-153">ホスト ・ デバイスの管理デバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="d6578-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="d6578-154">ホスト ・ デバイスが管理されている場合にも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d6578-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="d6578-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d6578-155">azureADDeviceId</span></span>|<span data-ttu-id="d6578-156">String</span><span class="sxs-lookup"><span data-stu-id="d6578-156">String</span></span>|<span data-ttu-id="d6578-157">ホスト ・ デバイスの Azure Active Directory のデバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="d6578-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="d6578-158">ホスト ・ デバイスは、Azure Active Directory が登録されている場合でも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d6578-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="d6578-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d6578-159">deviceModel</span></span>|<span data-ttu-id="d6578-160">String</span><span class="sxs-lookup"><span data-stu-id="d6578-160">String</span></span>|<span data-ttu-id="d6578-161">現在のアプリケーションの登録用のデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="d6578-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="d6578-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="d6578-162">deviceManufacturer</span></span>|<span data-ttu-id="d6578-163">String</span><span class="sxs-lookup"><span data-stu-id="d6578-163">String</span></span>|<span data-ttu-id="d6578-164">現在のアプリケーションの登録のためのデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="d6578-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="d6578-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d6578-165">flaggedReasons</span></span>|<span data-ttu-id="d6578-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d6578-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d6578-167">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="d6578-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d6578-168">例:</span><span class="sxs-lookup"><span data-stu-id="d6578-168">E.g.</span></span> <span data-ttu-id="d6578-169">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="d6578-169">app running on rooted device</span></span>|
|<span data-ttu-id="d6578-170">userId</span><span class="sxs-lookup"><span data-stu-id="d6578-170">userId</span></span>|<span data-ttu-id="d6578-171">String</span><span class="sxs-lookup"><span data-stu-id="d6578-171">String</span></span>|<span data-ttu-id="d6578-172">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="d6578-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="d6578-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6578-173">appIdentifier</span></span>|[<span data-ttu-id="d6578-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6578-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d6578-175">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="d6578-175">The app package Identifier</span></span>|
|<span data-ttu-id="d6578-176">id</span><span class="sxs-lookup"><span data-stu-id="d6578-176">id</span></span>|<span data-ttu-id="d6578-177">String</span><span class="sxs-lookup"><span data-stu-id="d6578-177">String</span></span>|<span data-ttu-id="d6578-178">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d6578-178">Key of the entity.</span></span>|
|<span data-ttu-id="d6578-179">version</span><span class="sxs-lookup"><span data-stu-id="d6578-179">version</span></span>|<span data-ttu-id="d6578-180">String</span><span class="sxs-lookup"><span data-stu-id="d6578-180">String</span></span>|<span data-ttu-id="d6578-181">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d6578-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6578-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6578-182">Relationships</span></span>
|<span data-ttu-id="d6578-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6578-183">Relationship</span></span>|<span data-ttu-id="d6578-184">型</span><span class="sxs-lookup"><span data-stu-id="d6578-184">Type</span></span>|<span data-ttu-id="d6578-185">説明</span><span class="sxs-lookup"><span data-stu-id="d6578-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6578-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d6578-186">appliedPolicies</span></span>|<span data-ttu-id="d6578-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d6578-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d6578-188">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="d6578-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="d6578-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="d6578-189">intendedPolicies</span></span>|<span data-ttu-id="d6578-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d6578-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d6578-191">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="d6578-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="d6578-192">operations</span><span class="sxs-lookup"><span data-stu-id="d6578-192">operations</span></span>|<span data-ttu-id="d6578-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d6578-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d6578-194">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="d6578-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6578-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6578-195">JSON Representation</span></span>
<span data-ttu-id="d6578-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d6578-196">Here is a JSON representation of the resource.</span></span>
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





