---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2a971b4e03da4dfdac6dfcdf621715db3e3d1e1
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36374037"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="f15b5-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="f15b5-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="f15b5-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f15b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f15b5-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f15b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f15b5-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="f15b5-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="f15b5-108">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="f15b5-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="f15b5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f15b5-109">Methods</span></span>
|<span data-ttu-id="f15b5-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f15b5-110">Method</span></span>|<span data-ttu-id="f15b5-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f15b5-111">Return Type</span></span>|<span data-ttu-id="f15b5-112">説明</span><span class="sxs-lookup"><span data-stu-id="f15b5-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f15b5-113">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="f15b5-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="f15b5-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f15b5-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="f15b5-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f15b5-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="f15b5-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f15b5-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="f15b5-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="f15b5-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="f15b5-118">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f15b5-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="f15b5-119">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="f15b5-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="f15b5-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f15b5-120">String collection</span></span>|<span data-ttu-id="f15b5-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f15b5-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f15b5-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f15b5-122">Properties</span></span>
|<span data-ttu-id="f15b5-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f15b5-123">Property</span></span>|<span data-ttu-id="f15b5-124">型</span><span class="sxs-lookup"><span data-stu-id="f15b5-124">Type</span></span>|<span data-ttu-id="f15b5-125">説明</span><span class="sxs-lookup"><span data-stu-id="f15b5-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f15b5-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f15b5-126">createdDateTime</span></span>|<span data-ttu-id="f15b5-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f15b5-127">DateTimeOffset</span></span>|<span data-ttu-id="f15b5-128">作成日時</span><span class="sxs-lookup"><span data-stu-id="f15b5-128">Date and time of creation</span></span>|
|<span data-ttu-id="f15b5-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f15b5-129">lastSyncDateTime</span></span>|<span data-ttu-id="f15b5-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f15b5-130">DateTimeOffset</span></span>|<span data-ttu-id="f15b5-131">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="f15b5-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="f15b5-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="f15b5-132">applicationVersion</span></span>|<span data-ttu-id="f15b5-133">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-133">String</span></span>|<span data-ttu-id="f15b5-134">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="f15b5-134">App version</span></span>|
|<span data-ttu-id="f15b5-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="f15b5-135">managementSdkVersion</span></span>|<span data-ttu-id="f15b5-136">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-136">String</span></span>|<span data-ttu-id="f15b5-137">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="f15b5-137">App management SDK version</span></span>|
|<span data-ttu-id="f15b5-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="f15b5-138">platformVersion</span></span>|<span data-ttu-id="f15b5-139">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-139">String</span></span>|<span data-ttu-id="f15b5-140">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="f15b5-140">Operating System version</span></span>|
|<span data-ttu-id="f15b5-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="f15b5-141">deviceType</span></span>|<span data-ttu-id="f15b5-142">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-142">String</span></span>|<span data-ttu-id="f15b5-143">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="f15b5-143">Host device type</span></span>|
|<span data-ttu-id="f15b5-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="f15b5-144">deviceTag</span></span>|<span data-ttu-id="f15b5-145">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-145">String</span></span>|<span data-ttu-id="f15b5-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="f15b5-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="f15b5-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="f15b5-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="f15b5-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="f15b5-148">deviceName</span></span>|<span data-ttu-id="f15b5-149">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-149">String</span></span>|<span data-ttu-id="f15b5-150">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="f15b5-150">Host device name</span></span>|
|<span data-ttu-id="f15b5-151">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f15b5-151">managedDeviceId</span></span>|<span data-ttu-id="f15b5-152">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-152">String</span></span>|<span data-ttu-id="f15b5-153">ホストデバイスの管理デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="f15b5-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="f15b5-154">ホストデバイスが管理されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f15b5-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="f15b5-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="f15b5-155">azureADDeviceId</span></span>|<span data-ttu-id="f15b5-156">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-156">String</span></span>|<span data-ttu-id="f15b5-157">ホストデバイスの Azure Active Directory デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="f15b5-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="f15b5-158">ホストデバイスが Azure Active Directory に登録されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f15b5-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="f15b5-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="f15b5-159">deviceModel</span></span>|<span data-ttu-id="f15b5-160">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-160">String</span></span>|<span data-ttu-id="f15b5-161">現在のアプリ登録のデバイスモデル</span><span class="sxs-lookup"><span data-stu-id="f15b5-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="f15b5-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="f15b5-162">deviceManufacturer</span></span>|<span data-ttu-id="f15b5-163">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-163">String</span></span>|<span data-ttu-id="f15b5-164">現在のアプリ登録のデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="f15b5-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="f15b5-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="f15b5-165">flaggedReasons</span></span>|<span data-ttu-id="f15b5-166">[Managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f15b5-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="f15b5-167">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="f15b5-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="f15b5-168">例:</span><span class="sxs-lookup"><span data-stu-id="f15b5-168">E.g.</span></span> <span data-ttu-id="f15b5-169">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="f15b5-169">app running on rooted device</span></span>|
|<span data-ttu-id="f15b5-170">userId</span><span class="sxs-lookup"><span data-stu-id="f15b5-170">userId</span></span>|<span data-ttu-id="f15b5-171">String</span><span class="sxs-lookup"><span data-stu-id="f15b5-171">String</span></span>|<span data-ttu-id="f15b5-172">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="f15b5-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="f15b5-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="f15b5-173">appIdentifier</span></span>|[<span data-ttu-id="f15b5-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="f15b5-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="f15b5-175">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="f15b5-175">The app package Identifier</span></span>|
|<span data-ttu-id="f15b5-176">id</span><span class="sxs-lookup"><span data-stu-id="f15b5-176">id</span></span>|<span data-ttu-id="f15b5-177">文字列</span><span class="sxs-lookup"><span data-stu-id="f15b5-177">String</span></span>|<span data-ttu-id="f15b5-178">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f15b5-178">Key of the entity.</span></span>|
|<span data-ttu-id="f15b5-179">version</span><span class="sxs-lookup"><span data-stu-id="f15b5-179">version</span></span>|<span data-ttu-id="f15b5-180">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f15b5-180">String</span></span>|<span data-ttu-id="f15b5-181">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f15b5-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f15b5-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f15b5-182">Relationships</span></span>
|<span data-ttu-id="f15b5-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f15b5-183">Relationship</span></span>|<span data-ttu-id="f15b5-184">型</span><span class="sxs-lookup"><span data-stu-id="f15b5-184">Type</span></span>|<span data-ttu-id="f15b5-185">説明</span><span class="sxs-lookup"><span data-stu-id="f15b5-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f15b5-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="f15b5-186">appliedPolicies</span></span>|<span data-ttu-id="f15b5-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f15b5-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f15b5-188">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="f15b5-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="f15b5-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="f15b5-189">intendedPolicies</span></span>|<span data-ttu-id="f15b5-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f15b5-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="f15b5-191">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="f15b5-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="f15b5-192">operations</span><span class="sxs-lookup"><span data-stu-id="f15b5-192">operations</span></span>|<span data-ttu-id="f15b5-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f15b5-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="f15b5-194">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="f15b5-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f15b5-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f15b5-195">JSON Representation</span></span>
<span data-ttu-id="f15b5-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f15b5-196">Here is a JSON representation of the resource.</span></span>
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



