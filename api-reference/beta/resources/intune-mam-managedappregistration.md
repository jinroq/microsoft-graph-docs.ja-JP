---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5532b4feaeaedd631c6e561f9e68722cba47a14
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940702"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="fbcaf-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="fbcaf-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="fbcaf-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbcaf-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbcaf-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="fbcaf-108">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="fbcaf-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbcaf-109">Methods</span></span>
|<span data-ttu-id="fbcaf-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="fbcaf-110">Method</span></span>|<span data-ttu-id="fbcaf-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fbcaf-111">Return Type</span></span>|<span data-ttu-id="fbcaf-112">説明</span><span class="sxs-lookup"><span data-stu-id="fbcaf-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fbcaf-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="fbcaf-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="fbcaf-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbcaf-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="fbcaf-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="fbcaf-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fbcaf-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="fbcaf-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="fbcaf-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="fbcaf-118">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="fbcaf-119">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="fbcaf-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="fbcaf-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fbcaf-120">String collection</span></span>|<span data-ttu-id="fbcaf-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fbcaf-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="fbcaf-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbcaf-122">Properties</span></span>
|<span data-ttu-id="fbcaf-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fbcaf-123">Property</span></span>|<span data-ttu-id="fbcaf-124">種類</span><span class="sxs-lookup"><span data-stu-id="fbcaf-124">Type</span></span>|<span data-ttu-id="fbcaf-125">説明</span><span class="sxs-lookup"><span data-stu-id="fbcaf-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbcaf-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fbcaf-126">createdDateTime</span></span>|<span data-ttu-id="fbcaf-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbcaf-127">DateTimeOffset</span></span>|<span data-ttu-id="fbcaf-128">作成日時</span><span class="sxs-lookup"><span data-stu-id="fbcaf-128">Date and time of creation</span></span>|
|<span data-ttu-id="fbcaf-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="fbcaf-129">lastSyncDateTime</span></span>|<span data-ttu-id="fbcaf-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fbcaf-130">DateTimeOffset</span></span>|<span data-ttu-id="fbcaf-131">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="fbcaf-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="fbcaf-132">applicationVersion</span></span>|<span data-ttu-id="fbcaf-133">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-133">String</span></span>|<span data-ttu-id="fbcaf-134">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="fbcaf-134">App version</span></span>|
|<span data-ttu-id="fbcaf-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="fbcaf-135">managementSdkVersion</span></span>|<span data-ttu-id="fbcaf-136">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-136">String</span></span>|<span data-ttu-id="fbcaf-137">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="fbcaf-137">App management SDK version</span></span>|
|<span data-ttu-id="fbcaf-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="fbcaf-138">platformVersion</span></span>|<span data-ttu-id="fbcaf-139">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-139">String</span></span>|<span data-ttu-id="fbcaf-140">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="fbcaf-140">Operating System version</span></span>|
|<span data-ttu-id="fbcaf-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="fbcaf-141">deviceType</span></span>|<span data-ttu-id="fbcaf-142">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-142">String</span></span>|<span data-ttu-id="fbcaf-143">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="fbcaf-143">Host device type</span></span>|
|<span data-ttu-id="fbcaf-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="fbcaf-144">deviceTag</span></span>|<span data-ttu-id="fbcaf-145">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-145">String</span></span>|<span data-ttu-id="fbcaf-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="fbcaf-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="fbcaf-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="fbcaf-148">deviceName</span></span>|<span data-ttu-id="fbcaf-149">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-149">String</span></span>|<span data-ttu-id="fbcaf-150">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="fbcaf-150">Host device name</span></span>|
|<span data-ttu-id="fbcaf-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="fbcaf-151">managedDeviceId</span></span>|<span data-ttu-id="fbcaf-152">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-152">String</span></span>|<span data-ttu-id="fbcaf-153">ホストデバイスの管理デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="fbcaf-154">ホストデバイスが管理されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="fbcaf-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="fbcaf-155">azureADDeviceId</span></span>|<span data-ttu-id="fbcaf-156">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-156">String</span></span>|<span data-ttu-id="fbcaf-157">ホストデバイスの Azure Active Directory デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="fbcaf-158">ホストデバイスが Azure Active Directory に登録されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="fbcaf-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="fbcaf-159">deviceModel</span></span>|<span data-ttu-id="fbcaf-160">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-160">String</span></span>|<span data-ttu-id="fbcaf-161">現在のアプリ登録のデバイスモデル</span><span class="sxs-lookup"><span data-stu-id="fbcaf-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="fbcaf-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="fbcaf-162">deviceManufacturer</span></span>|<span data-ttu-id="fbcaf-163">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-163">String</span></span>|<span data-ttu-id="fbcaf-164">現在のアプリ登録のデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="fbcaf-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="fbcaf-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="fbcaf-165">flaggedReasons</span></span>|<span data-ttu-id="fbcaf-166">[Managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="fbcaf-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="fbcaf-167">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="fbcaf-168">例:</span><span class="sxs-lookup"><span data-stu-id="fbcaf-168">E.g.</span></span> <span data-ttu-id="fbcaf-169">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="fbcaf-169">app running on rooted device</span></span>|
|<span data-ttu-id="fbcaf-170">userId</span><span class="sxs-lookup"><span data-stu-id="fbcaf-170">userId</span></span>|<span data-ttu-id="fbcaf-171">String</span><span class="sxs-lookup"><span data-stu-id="fbcaf-171">String</span></span>|<span data-ttu-id="fbcaf-172">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="fbcaf-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="fbcaf-173">appIdentifier</span></span>|[<span data-ttu-id="fbcaf-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="fbcaf-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="fbcaf-175">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="fbcaf-175">The app package Identifier</span></span>|
|<span data-ttu-id="fbcaf-176">id</span><span class="sxs-lookup"><span data-stu-id="fbcaf-176">id</span></span>|<span data-ttu-id="fbcaf-177">文字列</span><span class="sxs-lookup"><span data-stu-id="fbcaf-177">String</span></span>|<span data-ttu-id="fbcaf-178">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-178">Key of the entity.</span></span>|
|<span data-ttu-id="fbcaf-179">version</span><span class="sxs-lookup"><span data-stu-id="fbcaf-179">version</span></span>|<span data-ttu-id="fbcaf-180">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="fbcaf-180">String</span></span>|<span data-ttu-id="fbcaf-181">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fbcaf-182">関係</span><span class="sxs-lookup"><span data-stu-id="fbcaf-182">Relationships</span></span>
|<span data-ttu-id="fbcaf-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fbcaf-183">Relationship</span></span>|<span data-ttu-id="fbcaf-184">型</span><span class="sxs-lookup"><span data-stu-id="fbcaf-184">Type</span></span>|<span data-ttu-id="fbcaf-185">説明</span><span class="sxs-lookup"><span data-stu-id="fbcaf-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbcaf-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="fbcaf-186">appliedPolicies</span></span>|<span data-ttu-id="fbcaf-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbcaf-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="fbcaf-188">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="fbcaf-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="fbcaf-189">intendedPolicies</span></span>|<span data-ttu-id="fbcaf-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbcaf-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="fbcaf-191">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="fbcaf-192">operations</span><span class="sxs-lookup"><span data-stu-id="fbcaf-192">operations</span></span>|<span data-ttu-id="fbcaf-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fbcaf-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="fbcaf-194">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fbcaf-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fbcaf-195">JSON Representation</span></span>
<span data-ttu-id="fbcaf-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fbcaf-196">Here is a JSON representation of the resource.</span></span>
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




