---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a7b10a7d960c449aee4f911f4992955bde18724
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037913"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="c9da5-104">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c9da5-104">managedAppRegistration resource type</span></span>

> <span data-ttu-id="c9da5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9da5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9da5-106">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="c9da5-106">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="c9da5-107">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="c9da5-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="c9da5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9da5-108">Methods</span></span>
|<span data-ttu-id="c9da5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c9da5-109">Method</span></span>|<span data-ttu-id="c9da5-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c9da5-110">Return Type</span></span>|<span data-ttu-id="c9da5-111">説明</span><span class="sxs-lookup"><span data-stu-id="c9da5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c9da5-112">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c9da5-112">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="c9da5-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9da5-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="c9da5-114">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c9da5-114">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="c9da5-115">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c9da5-115">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="c9da5-116">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c9da5-116">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="c9da5-117">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c9da5-117">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="c9da5-118">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="c9da5-118">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="c9da5-119">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c9da5-119">String collection</span></span>|<span data-ttu-id="c9da5-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c9da5-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c9da5-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9da5-121">Properties</span></span>
|<span data-ttu-id="c9da5-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9da5-122">Property</span></span>|<span data-ttu-id="c9da5-123">型</span><span class="sxs-lookup"><span data-stu-id="c9da5-123">Type</span></span>|<span data-ttu-id="c9da5-124">説明</span><span class="sxs-lookup"><span data-stu-id="c9da5-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9da5-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9da5-125">createdDateTime</span></span>|<span data-ttu-id="c9da5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9da5-126">DateTimeOffset</span></span>|<span data-ttu-id="c9da5-127">作成日時</span><span class="sxs-lookup"><span data-stu-id="c9da5-127">Date and time of creation</span></span>|
|<span data-ttu-id="c9da5-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c9da5-128">lastSyncDateTime</span></span>|<span data-ttu-id="c9da5-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9da5-129">DateTimeOffset</span></span>|<span data-ttu-id="c9da5-130">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c9da5-130">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="c9da5-131">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c9da5-131">applicationVersion</span></span>|<span data-ttu-id="c9da5-132">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-132">String</span></span>|<span data-ttu-id="c9da5-133">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="c9da5-133">App version</span></span>|
|<span data-ttu-id="c9da5-134">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c9da5-134">managementSdkVersion</span></span>|<span data-ttu-id="c9da5-135">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-135">String</span></span>|<span data-ttu-id="c9da5-136">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="c9da5-136">App management SDK version</span></span>|
|<span data-ttu-id="c9da5-137">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c9da5-137">platformVersion</span></span>|<span data-ttu-id="c9da5-138">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-138">String</span></span>|<span data-ttu-id="c9da5-139">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="c9da5-139">Operating System version</span></span>|
|<span data-ttu-id="c9da5-140">deviceType</span><span class="sxs-lookup"><span data-stu-id="c9da5-140">deviceType</span></span>|<span data-ttu-id="c9da5-141">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-141">String</span></span>|<span data-ttu-id="c9da5-142">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="c9da5-142">Host device type</span></span>|
|<span data-ttu-id="c9da5-143">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c9da5-143">deviceTag</span></span>|<span data-ttu-id="c9da5-144">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-144">String</span></span>|<span data-ttu-id="c9da5-145">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="c9da5-145">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c9da5-146">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="c9da5-146">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="c9da5-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="c9da5-147">deviceName</span></span>|<span data-ttu-id="c9da5-148">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-148">String</span></span>|<span data-ttu-id="c9da5-149">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="c9da5-149">Host device name</span></span>|
|<span data-ttu-id="c9da5-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c9da5-150">flaggedReasons</span></span>|<span data-ttu-id="c9da5-151">[Managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c9da5-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c9da5-152">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="c9da5-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c9da5-153">例:</span><span class="sxs-lookup"><span data-stu-id="c9da5-153">E.g.</span></span> <span data-ttu-id="c9da5-154">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="c9da5-154">app running on rooted device</span></span>|
|<span data-ttu-id="c9da5-155">userId</span><span class="sxs-lookup"><span data-stu-id="c9da5-155">userId</span></span>|<span data-ttu-id="c9da5-156">String</span><span class="sxs-lookup"><span data-stu-id="c9da5-156">String</span></span>|<span data-ttu-id="c9da5-157">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="c9da5-157">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="c9da5-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9da5-158">appIdentifier</span></span>|[<span data-ttu-id="c9da5-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9da5-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c9da5-160">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="c9da5-160">The app package Identifier</span></span>|
|<span data-ttu-id="c9da5-161">id</span><span class="sxs-lookup"><span data-stu-id="c9da5-161">id</span></span>|<span data-ttu-id="c9da5-162">文字列</span><span class="sxs-lookup"><span data-stu-id="c9da5-162">String</span></span>|<span data-ttu-id="c9da5-163">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c9da5-163">Key of the entity.</span></span>|
|<span data-ttu-id="c9da5-164">version</span><span class="sxs-lookup"><span data-stu-id="c9da5-164">version</span></span>|<span data-ttu-id="c9da5-165">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c9da5-165">String</span></span>|<span data-ttu-id="c9da5-166">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c9da5-166">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9da5-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9da5-167">Relationships</span></span>
|<span data-ttu-id="c9da5-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9da5-168">Relationship</span></span>|<span data-ttu-id="c9da5-169">型</span><span class="sxs-lookup"><span data-stu-id="c9da5-169">Type</span></span>|<span data-ttu-id="c9da5-170">説明</span><span class="sxs-lookup"><span data-stu-id="c9da5-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9da5-171">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c9da5-171">appliedPolicies</span></span>|<span data-ttu-id="c9da5-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9da5-172">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c9da5-173">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c9da5-173">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="c9da5-174">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="c9da5-174">intendedPolicies</span></span>|<span data-ttu-id="c9da5-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9da5-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c9da5-176">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c9da5-176">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="c9da5-177">operations</span><span class="sxs-lookup"><span data-stu-id="c9da5-177">operations</span></span>|<span data-ttu-id="c9da5-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c9da5-178">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="c9da5-179">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="c9da5-179">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9da5-180">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9da5-180">JSON Representation</span></span>
<span data-ttu-id="c9da5-181">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9da5-181">Here is a JSON representation of the resource.</span></span>
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


