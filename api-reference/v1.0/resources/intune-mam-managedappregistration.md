---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 559ce934cf669241d4bee1db4e740d7806020f94
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345758"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="21bb7-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="21bb7-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="21bb7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21bb7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21bb7-106">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="21bb7-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="21bb7-107">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="21bb7-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="21bb7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="21bb7-108">Methods</span></span>
|<span data-ttu-id="21bb7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="21bb7-109">Method</span></span>|<span data-ttu-id="21bb7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21bb7-110">Return Type</span></span>|<span data-ttu-id="21bb7-111">説明</span><span class="sxs-lookup"><span data-stu-id="21bb7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="21bb7-112">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="21bb7-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="21bb7-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21bb7-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="21bb7-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="21bb7-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="21bb7-115">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="21bb7-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="21bb7-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="21bb7-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="21bb7-117">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="21bb7-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="21bb7-118">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="21bb7-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="21bb7-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="21bb7-119">String collection</span></span>|<span data-ttu-id="21bb7-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="21bb7-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="21bb7-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21bb7-121">Properties</span></span>
|<span data-ttu-id="21bb7-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21bb7-122">Property</span></span>|<span data-ttu-id="21bb7-123">型</span><span class="sxs-lookup"><span data-stu-id="21bb7-123">Type</span></span>|<span data-ttu-id="21bb7-124">説明</span><span class="sxs-lookup"><span data-stu-id="21bb7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bb7-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21bb7-125">createdDateTime</span></span>|<span data-ttu-id="21bb7-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21bb7-126">DateTimeOffset</span></span>|<span data-ttu-id="21bb7-127">作成日時</span><span class="sxs-lookup"><span data-stu-id="21bb7-127">Date and time of creation</span></span>|
|<span data-ttu-id="21bb7-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="21bb7-128">lastSyncDateTime</span></span>|<span data-ttu-id="21bb7-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21bb7-129">DateTimeOffset</span></span>|<span data-ttu-id="21bb7-130">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="21bb7-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="21bb7-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="21bb7-131">applicationVersion</span></span>|<span data-ttu-id="21bb7-132">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-132">String</span></span>|<span data-ttu-id="21bb7-133">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="21bb7-133">App version</span></span>|
|<span data-ttu-id="21bb7-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="21bb7-134">managementSdkVersion</span></span>|<span data-ttu-id="21bb7-135">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-135">String</span></span>|<span data-ttu-id="21bb7-136">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="21bb7-136">App management SDK version</span></span>|
|<span data-ttu-id="21bb7-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="21bb7-137">platformVersion</span></span>|<span data-ttu-id="21bb7-138">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-138">String</span></span>|<span data-ttu-id="21bb7-139">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="21bb7-139">Operating System version</span></span>|
|<span data-ttu-id="21bb7-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="21bb7-140">deviceType</span></span>|<span data-ttu-id="21bb7-141">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-141">String</span></span>|<span data-ttu-id="21bb7-142">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="21bb7-142">Host device type</span></span>|
|<span data-ttu-id="21bb7-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="21bb7-143">deviceTag</span></span>|<span data-ttu-id="21bb7-144">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-144">String</span></span>|<span data-ttu-id="21bb7-145">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="21bb7-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="21bb7-146">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="21bb7-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="21bb7-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="21bb7-147">deviceName</span></span>|<span data-ttu-id="21bb7-148">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-148">String</span></span>|<span data-ttu-id="21bb7-149">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="21bb7-149">Host device name</span></span>|
|<span data-ttu-id="21bb7-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="21bb7-150">flaggedReasons</span></span>|<span data-ttu-id="21bb7-151">[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="21bb7-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="21bb7-152">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="21bb7-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="21bb7-153">例:</span><span class="sxs-lookup"><span data-stu-id="21bb7-153">E.g.</span></span> <span data-ttu-id="21bb7-154">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="21bb7-154">app running on rooted device</span></span>|
|<span data-ttu-id="21bb7-155">userId</span><span class="sxs-lookup"><span data-stu-id="21bb7-155">userId</span></span>|<span data-ttu-id="21bb7-156">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-156">String</span></span>|<span data-ttu-id="21bb7-157">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="21bb7-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="21bb7-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="21bb7-158">appIdentifier</span></span>|[<span data-ttu-id="21bb7-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="21bb7-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="21bb7-160">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="21bb7-160">The app package Identifier</span></span>|
|<span data-ttu-id="21bb7-161">id</span><span class="sxs-lookup"><span data-stu-id="21bb7-161">id</span></span>|<span data-ttu-id="21bb7-162">String</span><span class="sxs-lookup"><span data-stu-id="21bb7-162">String</span></span>|<span data-ttu-id="21bb7-163">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="21bb7-163">Key of the entity.</span></span>|
|<span data-ttu-id="21bb7-164">version</span><span class="sxs-lookup"><span data-stu-id="21bb7-164">version</span></span>|<span data-ttu-id="21bb7-165">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="21bb7-165">String</span></span>|<span data-ttu-id="21bb7-166">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="21bb7-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21bb7-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21bb7-167">Relationships</span></span>
|<span data-ttu-id="21bb7-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21bb7-168">Relationship</span></span>|<span data-ttu-id="21bb7-169">型</span><span class="sxs-lookup"><span data-stu-id="21bb7-169">Type</span></span>|<span data-ttu-id="21bb7-170">説明</span><span class="sxs-lookup"><span data-stu-id="21bb7-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21bb7-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="21bb7-171">appliedPolicies</span></span>|<span data-ttu-id="21bb7-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21bb7-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="21bb7-173">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="21bb7-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="21bb7-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="21bb7-174">intendedPolicies</span></span>|<span data-ttu-id="21bb7-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21bb7-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="21bb7-176">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="21bb7-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="21bb7-177">operations</span><span class="sxs-lookup"><span data-stu-id="21bb7-177">operations</span></span>|<span data-ttu-id="21bb7-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21bb7-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="21bb7-179">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="21bb7-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21bb7-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21bb7-180">JSON Representation</span></span>
<span data-ttu-id="21bb7-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21bb7-181">Here is a JSON representation of the resource.</span></span>
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

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappregistration.md/microsoft.graph.managedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


