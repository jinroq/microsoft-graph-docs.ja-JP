---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
ms.openlocfilehash: 218a36a283febe646afcc6f9c9bcbd0ed5abf46a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347790"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="c64a7-103">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c64a7-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="c64a7-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c64a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c64a7-105">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="c64a7-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="c64a7-106">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="c64a7-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="c64a7-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c64a7-107">Methods</span></span>
|<span data-ttu-id="c64a7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c64a7-108">Method</span></span>|<span data-ttu-id="c64a7-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c64a7-109">Return Type</span></span>|<span data-ttu-id="c64a7-110">説明</span><span class="sxs-lookup"><span data-stu-id="c64a7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c64a7-111">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c64a7-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="c64a7-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c64a7-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="c64a7-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c64a7-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="c64a7-114">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c64a7-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="c64a7-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c64a7-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="c64a7-116">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c64a7-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="c64a7-117">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="c64a7-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="c64a7-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c64a7-118">String collection</span></span>|<span data-ttu-id="c64a7-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c64a7-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c64a7-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c64a7-120">Properties</span></span>
|<span data-ttu-id="c64a7-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c64a7-121">Property</span></span>|<span data-ttu-id="c64a7-122">種類</span><span class="sxs-lookup"><span data-stu-id="c64a7-122">Type</span></span>|<span data-ttu-id="c64a7-123">説明</span><span class="sxs-lookup"><span data-stu-id="c64a7-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c64a7-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c64a7-124">createdDateTime</span></span>|<span data-ttu-id="c64a7-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c64a7-125">DateTimeOffset</span></span>|<span data-ttu-id="c64a7-126">作成日時</span><span class="sxs-lookup"><span data-stu-id="c64a7-126">Date and time of creation</span></span>|
|<span data-ttu-id="c64a7-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c64a7-127">lastSyncDateTime</span></span>|<span data-ttu-id="c64a7-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c64a7-128">DateTimeOffset</span></span>|<span data-ttu-id="c64a7-129">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c64a7-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="c64a7-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c64a7-130">applicationVersion</span></span>|<span data-ttu-id="c64a7-131">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-131">String</span></span>|<span data-ttu-id="c64a7-132">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="c64a7-132">App version</span></span>|
|<span data-ttu-id="c64a7-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c64a7-133">managementSdkVersion</span></span>|<span data-ttu-id="c64a7-134">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-134">String</span></span>|<span data-ttu-id="c64a7-135">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="c64a7-135">App management SDK version</span></span>|
|<span data-ttu-id="c64a7-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c64a7-136">platformVersion</span></span>|<span data-ttu-id="c64a7-137">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-137">String</span></span>|<span data-ttu-id="c64a7-138">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="c64a7-138">Operating System version</span></span>|
|<span data-ttu-id="c64a7-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="c64a7-139">deviceType</span></span>|<span data-ttu-id="c64a7-140">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-140">String</span></span>|<span data-ttu-id="c64a7-141">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="c64a7-141">Host device type</span></span>|
|<span data-ttu-id="c64a7-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c64a7-142">deviceTag</span></span>|<span data-ttu-id="c64a7-143">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-143">String</span></span>|<span data-ttu-id="c64a7-144">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="c64a7-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c64a7-145">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="c64a7-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="c64a7-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="c64a7-146">deviceName</span></span>|<span data-ttu-id="c64a7-147">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-147">String</span></span>|<span data-ttu-id="c64a7-148">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="c64a7-148">Host device name</span></span>|
|<span data-ttu-id="c64a7-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c64a7-149">flaggedReasons</span></span>|<span data-ttu-id="c64a7-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c64a7-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c64a7-151">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="c64a7-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c64a7-152">例:</span><span class="sxs-lookup"><span data-stu-id="c64a7-152">E.g.</span></span> <span data-ttu-id="c64a7-153">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="c64a7-153">app running on rooted device</span></span>|
|<span data-ttu-id="c64a7-154">userId</span><span class="sxs-lookup"><span data-stu-id="c64a7-154">userId</span></span>|<span data-ttu-id="c64a7-155">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-155">String</span></span>|<span data-ttu-id="c64a7-156">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="c64a7-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="c64a7-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c64a7-157">appIdentifier</span></span>|[<span data-ttu-id="c64a7-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c64a7-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c64a7-159">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="c64a7-159">The app package Identifier</span></span>|
|<span data-ttu-id="c64a7-160">id</span><span class="sxs-lookup"><span data-stu-id="c64a7-160">id</span></span>|<span data-ttu-id="c64a7-161">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-161">String</span></span>|<span data-ttu-id="c64a7-162">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c64a7-162">Key of the entity.</span></span>|
|<span data-ttu-id="c64a7-163">version</span><span class="sxs-lookup"><span data-stu-id="c64a7-163">version</span></span>|<span data-ttu-id="c64a7-164">String</span><span class="sxs-lookup"><span data-stu-id="c64a7-164">String</span></span>|<span data-ttu-id="c64a7-165">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c64a7-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c64a7-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c64a7-166">Relationships</span></span>
|<span data-ttu-id="c64a7-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c64a7-167">Relationship</span></span>|<span data-ttu-id="c64a7-168">型</span><span class="sxs-lookup"><span data-stu-id="c64a7-168">Type</span></span>|<span data-ttu-id="c64a7-169">説明</span><span class="sxs-lookup"><span data-stu-id="c64a7-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c64a7-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c64a7-170">appliedPolicies</span></span>|<span data-ttu-id="c64a7-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c64a7-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c64a7-172">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c64a7-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="c64a7-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="c64a7-173">intendedPolicies</span></span>|<span data-ttu-id="c64a7-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c64a7-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c64a7-175">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c64a7-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="c64a7-176">operations</span><span class="sxs-lookup"><span data-stu-id="c64a7-176">operations</span></span>|<span data-ttu-id="c64a7-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c64a7-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="c64a7-178">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="c64a7-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c64a7-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c64a7-179">JSON Representation</span></span>
<span data-ttu-id="c64a7-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c64a7-180">Here is a JSON representation of the resource.</span></span>
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
