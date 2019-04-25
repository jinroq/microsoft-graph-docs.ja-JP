---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be91dd094258f0bf998521c058f1c62659fbcc8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581031"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="8a5ec-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8a5ec-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="8a5ec-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a5ec-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a5ec-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="8a5ec-108">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="8a5ec-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a5ec-109">Methods</span></span>
|<span data-ttu-id="8a5ec-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a5ec-110">Method</span></span>|<span data-ttu-id="8a5ec-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a5ec-111">Return Type</span></span>|<span data-ttu-id="8a5ec-112">説明</span><span class="sxs-lookup"><span data-stu-id="8a5ec-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a5ec-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="8a5ec-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="8a5ec-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a5ec-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="8a5ec-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="8a5ec-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8a5ec-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="8a5ec-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="8a5ec-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="8a5ec-118">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="8a5ec-119">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="8a5ec-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="8a5ec-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8a5ec-120">String collection</span></span>|<span data-ttu-id="8a5ec-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8a5ec-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8a5ec-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a5ec-122">Properties</span></span>
|<span data-ttu-id="8a5ec-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a5ec-123">Property</span></span>|<span data-ttu-id="8a5ec-124">型</span><span class="sxs-lookup"><span data-stu-id="8a5ec-124">Type</span></span>|<span data-ttu-id="8a5ec-125">説明</span><span class="sxs-lookup"><span data-stu-id="8a5ec-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a5ec-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8a5ec-126">createdDateTime</span></span>|<span data-ttu-id="8a5ec-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a5ec-127">DateTimeOffset</span></span>|<span data-ttu-id="8a5ec-128">作成日時</span><span class="sxs-lookup"><span data-stu-id="8a5ec-128">Date and time of creation</span></span>|
|<span data-ttu-id="8a5ec-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8a5ec-129">lastSyncDateTime</span></span>|<span data-ttu-id="8a5ec-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a5ec-130">DateTimeOffset</span></span>|<span data-ttu-id="8a5ec-131">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="8a5ec-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="8a5ec-132">applicationVersion</span></span>|<span data-ttu-id="8a5ec-133">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-133">String</span></span>|<span data-ttu-id="8a5ec-134">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="8a5ec-134">App version</span></span>|
|<span data-ttu-id="8a5ec-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="8a5ec-135">managementSdkVersion</span></span>|<span data-ttu-id="8a5ec-136">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-136">String</span></span>|<span data-ttu-id="8a5ec-137">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="8a5ec-137">App management SDK version</span></span>|
|<span data-ttu-id="8a5ec-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="8a5ec-138">platformVersion</span></span>|<span data-ttu-id="8a5ec-139">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-139">String</span></span>|<span data-ttu-id="8a5ec-140">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="8a5ec-140">Operating System version</span></span>|
|<span data-ttu-id="8a5ec-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="8a5ec-141">deviceType</span></span>|<span data-ttu-id="8a5ec-142">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-142">String</span></span>|<span data-ttu-id="8a5ec-143">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="8a5ec-143">Host device type</span></span>|
|<span data-ttu-id="8a5ec-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="8a5ec-144">deviceTag</span></span>|<span data-ttu-id="8a5ec-145">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-145">String</span></span>|<span data-ttu-id="8a5ec-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="8a5ec-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="8a5ec-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="8a5ec-148">deviceName</span></span>|<span data-ttu-id="8a5ec-149">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-149">String</span></span>|<span data-ttu-id="8a5ec-150">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="8a5ec-150">Host device name</span></span>|
|<span data-ttu-id="8a5ec-151">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="8a5ec-151">managedDeviceId</span></span>|<span data-ttu-id="8a5ec-152">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-152">String</span></span>|<span data-ttu-id="8a5ec-153">ホストデバイスの管理デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="8a5ec-154">ホストデバイスが管理されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="8a5ec-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="8a5ec-155">azureADDeviceId</span></span>|<span data-ttu-id="8a5ec-156">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-156">String</span></span>|<span data-ttu-id="8a5ec-157">ホストデバイスの Azure Active Directory デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="8a5ec-158">ホストデバイスが Azure Active Directory に登録されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="8a5ec-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="8a5ec-159">deviceModel</span></span>|<span data-ttu-id="8a5ec-160">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-160">String</span></span>|<span data-ttu-id="8a5ec-161">現在のアプリ登録のデバイスモデル</span><span class="sxs-lookup"><span data-stu-id="8a5ec-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="8a5ec-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="8a5ec-162">deviceManufacturer</span></span>|<span data-ttu-id="8a5ec-163">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-163">String</span></span>|<span data-ttu-id="8a5ec-164">現在のアプリ登録のデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="8a5ec-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="8a5ec-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="8a5ec-165">flaggedReasons</span></span>|<span data-ttu-id="8a5ec-166">[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8a5ec-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="8a5ec-167">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="8a5ec-168">例:</span><span class="sxs-lookup"><span data-stu-id="8a5ec-168">E.g.</span></span> <span data-ttu-id="8a5ec-169">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="8a5ec-169">app running on rooted device</span></span>|
|<span data-ttu-id="8a5ec-170">userId</span><span class="sxs-lookup"><span data-stu-id="8a5ec-170">userId</span></span>|<span data-ttu-id="8a5ec-171">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-171">String</span></span>|<span data-ttu-id="8a5ec-172">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="8a5ec-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a5ec-173">appIdentifier</span></span>|[<span data-ttu-id="8a5ec-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8a5ec-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="8a5ec-175">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="8a5ec-175">The app package Identifier</span></span>|
|<span data-ttu-id="8a5ec-176">id</span><span class="sxs-lookup"><span data-stu-id="8a5ec-176">id</span></span>|<span data-ttu-id="8a5ec-177">String</span><span class="sxs-lookup"><span data-stu-id="8a5ec-177">String</span></span>|<span data-ttu-id="8a5ec-178">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-178">Key of the entity.</span></span>|
|<span data-ttu-id="8a5ec-179">version</span><span class="sxs-lookup"><span data-stu-id="8a5ec-179">version</span></span>|<span data-ttu-id="8a5ec-180">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8a5ec-180">String</span></span>|<span data-ttu-id="8a5ec-181">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8a5ec-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a5ec-182">Relationships</span></span>
|<span data-ttu-id="8a5ec-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8a5ec-183">Relationship</span></span>|<span data-ttu-id="8a5ec-184">型</span><span class="sxs-lookup"><span data-stu-id="8a5ec-184">Type</span></span>|<span data-ttu-id="8a5ec-185">説明</span><span class="sxs-lookup"><span data-stu-id="8a5ec-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a5ec-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="8a5ec-186">appliedPolicies</span></span>|<span data-ttu-id="8a5ec-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a5ec-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8a5ec-188">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="8a5ec-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="8a5ec-189">intendedPolicies</span></span>|<span data-ttu-id="8a5ec-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a5ec-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="8a5ec-191">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="8a5ec-192">operations</span><span class="sxs-lookup"><span data-stu-id="8a5ec-192">operations</span></span>|<span data-ttu-id="8a5ec-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a5ec-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="8a5ec-194">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a5ec-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a5ec-195">JSON Representation</span></span>
<span data-ttu-id="8a5ec-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8a5ec-196">Here is a JSON representation of the resource.</span></span>
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





