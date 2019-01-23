---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a343dba3df1274693449b8f7cbefd83b131138c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421439"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="d8603-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="d8603-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="d8603-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8603-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d8603-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8603-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d8603-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8603-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8603-108">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="d8603-108">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="d8603-109">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="d8603-109">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="d8603-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8603-110">Methods</span></span>
|<span data-ttu-id="d8603-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8603-111">Method</span></span>|<span data-ttu-id="d8603-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8603-112">Return Type</span></span>|<span data-ttu-id="d8603-113">説明</span><span class="sxs-lookup"><span data-stu-id="d8603-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d8603-114">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="d8603-114">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="d8603-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d8603-115">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="d8603-116">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d8603-116">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="d8603-117">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d8603-117">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="d8603-118">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d8603-118">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="d8603-119">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d8603-119">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="d8603-120">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="d8603-120">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="d8603-121">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d8603-121">String collection</span></span>|<span data-ttu-id="d8603-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d8603-122">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d8603-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8603-123">Properties</span></span>
|<span data-ttu-id="d8603-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8603-124">Property</span></span>|<span data-ttu-id="d8603-125">型</span><span class="sxs-lookup"><span data-stu-id="d8603-125">Type</span></span>|<span data-ttu-id="d8603-126">説明</span><span class="sxs-lookup"><span data-stu-id="d8603-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8603-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8603-127">createdDateTime</span></span>|<span data-ttu-id="d8603-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8603-128">DateTimeOffset</span></span>|<span data-ttu-id="d8603-129">作成日時</span><span class="sxs-lookup"><span data-stu-id="d8603-129">Date and time of creation</span></span>|
|<span data-ttu-id="d8603-130">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d8603-130">lastSyncDateTime</span></span>|<span data-ttu-id="d8603-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8603-131">DateTimeOffset</span></span>|<span data-ttu-id="d8603-132">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="d8603-132">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="d8603-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d8603-133">applicationVersion</span></span>|<span data-ttu-id="d8603-134">String</span><span class="sxs-lookup"><span data-stu-id="d8603-134">String</span></span>|<span data-ttu-id="d8603-135">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="d8603-135">App version</span></span>|
|<span data-ttu-id="d8603-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d8603-136">managementSdkVersion</span></span>|<span data-ttu-id="d8603-137">String</span><span class="sxs-lookup"><span data-stu-id="d8603-137">String</span></span>|<span data-ttu-id="d8603-138">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="d8603-138">App management SDK version</span></span>|
|<span data-ttu-id="d8603-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d8603-139">platformVersion</span></span>|<span data-ttu-id="d8603-140">String</span><span class="sxs-lookup"><span data-stu-id="d8603-140">String</span></span>|<span data-ttu-id="d8603-141">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="d8603-141">Operating System version</span></span>|
|<span data-ttu-id="d8603-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="d8603-142">deviceType</span></span>|<span data-ttu-id="d8603-143">String</span><span class="sxs-lookup"><span data-stu-id="d8603-143">String</span></span>|<span data-ttu-id="d8603-144">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="d8603-144">Host device type</span></span>|
|<span data-ttu-id="d8603-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d8603-145">deviceTag</span></span>|<span data-ttu-id="d8603-146">String</span><span class="sxs-lookup"><span data-stu-id="d8603-146">String</span></span>|<span data-ttu-id="d8603-147">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="d8603-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d8603-148">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="d8603-148">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="d8603-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="d8603-149">deviceName</span></span>|<span data-ttu-id="d8603-150">String</span><span class="sxs-lookup"><span data-stu-id="d8603-150">String</span></span>|<span data-ttu-id="d8603-151">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="d8603-151">Host device name</span></span>|
|<span data-ttu-id="d8603-152">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d8603-152">managedDeviceId</span></span>|<span data-ttu-id="d8603-153">String</span><span class="sxs-lookup"><span data-stu-id="d8603-153">String</span></span>|<span data-ttu-id="d8603-154">ホスト ・ デバイスの管理デバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="d8603-154">The Managed Device identifier of the host device.</span></span> <span data-ttu-id="d8603-155">ホスト ・ デバイスが管理されている場合にも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d8603-155">Value could be empty even when the host device is managed.</span></span>|
|<span data-ttu-id="d8603-156">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="d8603-156">azureADDeviceId</span></span>|<span data-ttu-id="d8603-157">String</span><span class="sxs-lookup"><span data-stu-id="d8603-157">String</span></span>|<span data-ttu-id="d8603-158">ホスト ・ デバイスの Azure Active Directory のデバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="d8603-158">The Azure Active Directory Device identifier of the host device.</span></span> <span data-ttu-id="d8603-159">ホスト ・ デバイスは、Azure Active Directory が登録されている場合でも、値を空にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d8603-159">Value could be empty even when the host device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="d8603-160">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d8603-160">deviceModel</span></span>|<span data-ttu-id="d8603-161">String</span><span class="sxs-lookup"><span data-stu-id="d8603-161">String</span></span>|<span data-ttu-id="d8603-162">現在のアプリケーションの登録用のデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="d8603-162">The device model for the current app registration</span></span> |
|<span data-ttu-id="d8603-163">deviceManufacturer</span><span class="sxs-lookup"><span data-stu-id="d8603-163">deviceManufacturer</span></span>|<span data-ttu-id="d8603-164">String</span><span class="sxs-lookup"><span data-stu-id="d8603-164">String</span></span>|<span data-ttu-id="d8603-165">現在のアプリケーションの登録のためのデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="d8603-165">The device manufacturer for the current app registration</span></span> |
|<span data-ttu-id="d8603-166">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d8603-166">flaggedReasons</span></span>|<span data-ttu-id="d8603-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d8603-167">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="d8603-168">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="d8603-168">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d8603-169">例:</span><span class="sxs-lookup"><span data-stu-id="d8603-169">E.g.</span></span> <span data-ttu-id="d8603-170">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="d8603-170">app running on rooted device</span></span>|
|<span data-ttu-id="d8603-171">userId</span><span class="sxs-lookup"><span data-stu-id="d8603-171">userId</span></span>|<span data-ttu-id="d8603-172">String</span><span class="sxs-lookup"><span data-stu-id="d8603-172">String</span></span>|<span data-ttu-id="d8603-173">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="d8603-173">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="d8603-174">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d8603-174">appIdentifier</span></span>|[<span data-ttu-id="d8603-175">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d8603-175">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="d8603-176">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="d8603-176">The app package Identifier</span></span>|
|<span data-ttu-id="d8603-177">id</span><span class="sxs-lookup"><span data-stu-id="d8603-177">id</span></span>|<span data-ttu-id="d8603-178">String</span><span class="sxs-lookup"><span data-stu-id="d8603-178">String</span></span>|<span data-ttu-id="d8603-179">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d8603-179">Key of the entity.</span></span>|
|<span data-ttu-id="d8603-180">version</span><span class="sxs-lookup"><span data-stu-id="d8603-180">version</span></span>|<span data-ttu-id="d8603-181">String</span><span class="sxs-lookup"><span data-stu-id="d8603-181">String</span></span>|<span data-ttu-id="d8603-182">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d8603-182">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8603-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8603-183">Relationships</span></span>
|<span data-ttu-id="d8603-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8603-184">Relationship</span></span>|<span data-ttu-id="d8603-185">型</span><span class="sxs-lookup"><span data-stu-id="d8603-185">Type</span></span>|<span data-ttu-id="d8603-186">説明</span><span class="sxs-lookup"><span data-stu-id="d8603-186">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8603-187">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="d8603-187">appliedPolicies</span></span>|<span data-ttu-id="d8603-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d8603-188">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d8603-189">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="d8603-189">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="d8603-190">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="d8603-190">intendedPolicies</span></span>|<span data-ttu-id="d8603-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d8603-191">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="d8603-192">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="d8603-192">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="d8603-193">operations</span><span class="sxs-lookup"><span data-stu-id="d8603-193">operations</span></span>|<span data-ttu-id="d8603-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d8603-194">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="d8603-195">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="d8603-195">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8603-196">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8603-196">JSON Representation</span></span>
<span data-ttu-id="d8603-197">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8603-197">Here is a JSON representation of the resource.</span></span>
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




