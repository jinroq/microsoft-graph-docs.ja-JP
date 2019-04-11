---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3be91dd094258f0bf998521c058f1c62659fbcc8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794387"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="e5a24-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="e5a24-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="e5a24-105">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5a24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5a24-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5a24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5a24-107">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="e5a24-107">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="e5a24-108">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="e5a24-108">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="e5a24-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5a24-109">Methods</span></span>
|<span data-ttu-id="e5a24-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5a24-110">Method</span></span>|<span data-ttu-id="e5a24-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5a24-111">Return Type</span></span>|<span data-ttu-id="e5a24-112">説明</span><span class="sxs-lookup"><span data-stu-id="e5a24-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5a24-113">managedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="e5a24-113">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="e5a24-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a24-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="e5a24-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e5a24-115">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="e5a24-116">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e5a24-116">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="e5a24-117">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="e5a24-117">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="e5a24-118">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e5a24-118">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="e5a24-119">getUserIdsWithFlaggedAppRegistration 関数</span><span class="sxs-lookup"><span data-stu-id="e5a24-119">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="e5a24-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a24-120">String collection</span></span>|<span data-ttu-id="e5a24-121">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e5a24-121">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e5a24-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5a24-122">Properties</span></span>
|<span data-ttu-id="e5a24-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5a24-123">Property</span></span>|<span data-ttu-id="e5a24-124">型</span><span class="sxs-lookup"><span data-stu-id="e5a24-124">Type</span></span>|<span data-ttu-id="e5a24-125">説明</span><span class="sxs-lookup"><span data-stu-id="e5a24-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5a24-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5a24-126">createdDateTime</span></span>|<span data-ttu-id="e5a24-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5a24-127">DateTimeOffset</span></span>|<span data-ttu-id="e5a24-128">作成日時</span><span class="sxs-lookup"><span data-stu-id="e5a24-128">Date and time of creation</span></span>|
|<span data-ttu-id="e5a24-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e5a24-129">lastSyncDateTime</span></span>|<span data-ttu-id="e5a24-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5a24-130">DateTimeOffset</span></span>|<span data-ttu-id="e5a24-131">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="e5a24-131">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="e5a24-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="e5a24-132">applicationVersion</span></span>|<span data-ttu-id="e5a24-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-133">String</span></span>|<span data-ttu-id="e5a24-134">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="e5a24-134">App version</span></span>|
|<span data-ttu-id="e5a24-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="e5a24-135">managementSdkVersion</span></span>|<span data-ttu-id="e5a24-136">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-136">String</span></span>|<span data-ttu-id="e5a24-137">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="e5a24-137">App management SDK version</span></span>|
|<span data-ttu-id="e5a24-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="e5a24-138">platformVersion</span></span>|<span data-ttu-id="e5a24-139">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-139">String</span></span>|<span data-ttu-id="e5a24-140">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="e5a24-140">Operating System version</span></span>|
|<span data-ttu-id="e5a24-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="e5a24-141">deviceType</span></span>|<span data-ttu-id="e5a24-142">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-142">String</span></span>|<span data-ttu-id="e5a24-143">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="e5a24-143">Host device type</span></span>|
|<span data-ttu-id="e5a24-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="e5a24-144">deviceTag</span></span>|<span data-ttu-id="e5a24-145">String</span><span class="sxs-lookup"><span data-stu-id="e5a24-145">String</span></span>|<span data-ttu-id="e5a24-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e5a24-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="e5a24-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="e5a24-147">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="e5a24-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="e5a24-148">deviceName</span></span>|<span data-ttu-id="e5a24-149">String</span><span class="sxs-lookup"><span data-stu-id="e5a24-149">String</span></span>|<span data-ttu-id="e5a24-150">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="e5a24-150">Host device name</span></span>|
|<span data-ttu-id="e5a24-151">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="e5a24-151">managedDeviceId</span></span>|<span data-ttu-id="e5a24-152">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-152">String</span></span>|<span data-ttu-id="e5a24-153">ホストデバイスの管理デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="e5a24-153">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="e5a24-154">ホストデバイスが管理されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5a24-154">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="e5a24-155">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="e5a24-155">azureADDeviceId</span></span>|<span data-ttu-id="e5a24-156">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-156">String</span></span>|<span data-ttu-id="e5a24-157">ホストデバイスの Azure Active Directory デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="e5a24-157">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="e5a24-158">ホストデバイスが Azure Active Directory に登録されている場合でも、値を空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e5a24-158">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="e5a24-159">deviceModel</span><span class="sxs-lookup"><span data-stu-id="e5a24-159">deviceModel</span></span>|<span data-ttu-id="e5a24-160">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-160">String</span></span>|<span data-ttu-id="e5a24-161">現在のアプリ登録のデバイスモデル</span><span class="sxs-lookup"><span data-stu-id="e5a24-161">The device model for the current app registration</span></span> |
|<span data-ttu-id="e5a24-162">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="e5a24-162">deviceManufacturer</span></span>|<span data-ttu-id="e5a24-163">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-163">String</span></span>|<span data-ttu-id="e5a24-164">現在のアプリ登録のデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="e5a24-164">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="e5a24-165">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="e5a24-165">flaggedReasons</span></span>|<span data-ttu-id="e5a24-166">[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a24-166">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="e5a24-167">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="e5a24-167">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="e5a24-168">例:</span><span class="sxs-lookup"><span data-stu-id="e5a24-168">E.g.</span></span> <span data-ttu-id="e5a24-169">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="e5a24-169">app running on rooted device</span></span>|
|<span data-ttu-id="e5a24-170">userId</span><span class="sxs-lookup"><span data-stu-id="e5a24-170">userId</span></span>|<span data-ttu-id="e5a24-171">文字列</span><span class="sxs-lookup"><span data-stu-id="e5a24-171">String</span></span>|<span data-ttu-id="e5a24-172">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="e5a24-172">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="e5a24-173">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e5a24-173">appIdentifier</span></span>|[<span data-ttu-id="e5a24-174">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="e5a24-174">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="e5a24-175">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="e5a24-175">The app package Identifier</span></span>|
|<span data-ttu-id="e5a24-176">id</span><span class="sxs-lookup"><span data-stu-id="e5a24-176">id</span></span>|<span data-ttu-id="e5a24-177">String</span><span class="sxs-lookup"><span data-stu-id="e5a24-177">String</span></span>|<span data-ttu-id="e5a24-178">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5a24-178">Key of the entity.</span></span>|
|<span data-ttu-id="e5a24-179">version</span><span class="sxs-lookup"><span data-stu-id="e5a24-179">version</span></span>|<span data-ttu-id="e5a24-180">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e5a24-180">String</span></span>|<span data-ttu-id="e5a24-181">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e5a24-181">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5a24-182">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5a24-182">Relationships</span></span>
|<span data-ttu-id="e5a24-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5a24-183">Relationship</span></span>|<span data-ttu-id="e5a24-184">型</span><span class="sxs-lookup"><span data-stu-id="e5a24-184">Type</span></span>|<span data-ttu-id="e5a24-185">説明</span><span class="sxs-lookup"><span data-stu-id="e5a24-185">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5a24-186">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="e5a24-186">appliedPolicies</span></span>|<span data-ttu-id="e5a24-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a24-187">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e5a24-188">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="e5a24-188">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="e5a24-189">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="e5a24-189">intendedPolicies</span></span>|<span data-ttu-id="e5a24-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a24-190">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="e5a24-191">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="e5a24-191">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="e5a24-192">operations</span><span class="sxs-lookup"><span data-stu-id="e5a24-192">operations</span></span>|<span data-ttu-id="e5a24-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5a24-193">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="e5a24-194">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="e5a24-194">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e5a24-195">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5a24-195">JSON Representation</span></span>
<span data-ttu-id="e5a24-196">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5a24-196">Here is a JSON representation of the resource.</span></span>
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





