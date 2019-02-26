---
title: androidManagedAppRegistration リソースの種類
description: 特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 047c9eaf29f96463e6493726b9d1815b3b2eaa01
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251686"
---
# <a name="androidmanagedappregistration-resource-type"></a><span data-ttu-id="feb3a-104">androidManagedAppRegistration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="feb3a-104">androidManagedAppRegistration resource type</span></span>

> <span data-ttu-id="feb3a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="feb3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="feb3a-106">特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。</span><span class="sxs-lookup"><span data-stu-id="feb3a-106">Represents the synchronization details of an android app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="feb3a-107">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="feb3a-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="feb3a-108">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-108">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="feb3a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="feb3a-109">Methods</span></span>
|<span data-ttu-id="feb3a-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="feb3a-110">Method</span></span>|<span data-ttu-id="feb3a-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="feb3a-111">Return Type</span></span>|<span data-ttu-id="feb3a-112">説明</span><span class="sxs-lookup"><span data-stu-id="feb3a-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="feb3a-113">androidManagedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="feb3a-113">List androidManagedAppRegistrations</span></span>](../api/intune-mam-androidmanagedappregistration-list.md)|<span data-ttu-id="feb3a-114">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="feb3a-114">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) collection</span></span>|<span data-ttu-id="feb3a-115">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="feb3a-115">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="feb3a-116">androidManagedAppRegistration の取得</span><span class="sxs-lookup"><span data-stu-id="feb3a-116">Get androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-get.md)|[<span data-ttu-id="feb3a-117">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="feb3a-117">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="feb3a-118">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="feb3a-118">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|
|[<span data-ttu-id="feb3a-119">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="feb3a-119">Create androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-create.md)|[<span data-ttu-id="feb3a-120">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="feb3a-120">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="feb3a-121">新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="feb3a-121">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="feb3a-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="feb3a-122">Properties</span></span>
|<span data-ttu-id="feb3a-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="feb3a-123">Property</span></span>|<span data-ttu-id="feb3a-124">型</span><span class="sxs-lookup"><span data-stu-id="feb3a-124">Type</span></span>|<span data-ttu-id="feb3a-125">説明</span><span class="sxs-lookup"><span data-stu-id="feb3a-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb3a-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="feb3a-126">createdDateTime</span></span>|<span data-ttu-id="feb3a-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feb3a-127">DateTimeOffset</span></span>|<span data-ttu-id="feb3a-128">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="feb3a-128">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-129">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="feb3a-129">lastSyncDateTime</span></span>|<span data-ttu-id="feb3a-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="feb3a-130">DateTimeOffset</span></span>|<span data-ttu-id="feb3a-131">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="feb3a-131">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="feb3a-132">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-132">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-133">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="feb3a-133">applicationVersion</span></span>|<span data-ttu-id="feb3a-134">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-134">String</span></span>|<span data-ttu-id="feb3a-135">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-135">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-136">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="feb3a-136">managementSdkVersion</span></span>|<span data-ttu-id="feb3a-137">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-137">String</span></span>|<span data-ttu-id="feb3a-138">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-138">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-139">platformVersion</span><span class="sxs-lookup"><span data-stu-id="feb3a-139">platformVersion</span></span>|<span data-ttu-id="feb3a-140">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-140">String</span></span>|<span data-ttu-id="feb3a-141">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-141">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-142">deviceType</span><span class="sxs-lookup"><span data-stu-id="feb3a-142">deviceType</span></span>|<span data-ttu-id="feb3a-143">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-143">String</span></span>|<span data-ttu-id="feb3a-144">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-144">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-145">deviceTag</span><span class="sxs-lookup"><span data-stu-id="feb3a-145">deviceTag</span></span>|<span data-ttu-id="feb3a-146">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-146">String</span></span>|<span data-ttu-id="feb3a-147">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="feb3a-147">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="feb3a-148">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="feb3a-148">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="feb3a-149">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-149">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-150">deviceName</span><span class="sxs-lookup"><span data-stu-id="feb3a-150">deviceName</span></span>|<span data-ttu-id="feb3a-151">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-151">String</span></span>|<span data-ttu-id="feb3a-152">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-152">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-153">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="feb3a-153">flaggedReasons</span></span>|<span data-ttu-id="feb3a-154">[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="feb3a-154">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="feb3a-155">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="feb3a-155">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="feb3a-156">例:</span><span class="sxs-lookup"><span data-stu-id="feb3a-156">E.g.</span></span> <span data-ttu-id="feb3a-157">ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-157">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-158">userId</span><span class="sxs-lookup"><span data-stu-id="feb3a-158">userId</span></span>|<span data-ttu-id="feb3a-159">String</span><span class="sxs-lookup"><span data-stu-id="feb3a-159">String</span></span>|<span data-ttu-id="feb3a-160">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="feb3a-160">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="feb3a-161">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-161">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-162">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="feb3a-162">appIdentifier</span></span>|[<span data-ttu-id="feb3a-163">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="feb3a-163">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="feb3a-164">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="feb3a-164">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-165">id</span><span class="sxs-lookup"><span data-stu-id="feb3a-165">id</span></span>|<span data-ttu-id="feb3a-166">文字列</span><span class="sxs-lookup"><span data-stu-id="feb3a-166">String</span></span>|<span data-ttu-id="feb3a-167">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="feb3a-167">Key of the entity.</span></span> <span data-ttu-id="feb3a-168">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-169">version</span><span class="sxs-lookup"><span data-stu-id="feb3a-169">version</span></span>|<span data-ttu-id="feb3a-170">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="feb3a-170">String</span></span>|<span data-ttu-id="feb3a-171">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="feb3a-171">Version of the entity.</span></span> <span data-ttu-id="feb3a-172">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-172">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="feb3a-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="feb3a-173">Relationships</span></span>
|<span data-ttu-id="feb3a-174">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="feb3a-174">Relationship</span></span>|<span data-ttu-id="feb3a-175">型</span><span class="sxs-lookup"><span data-stu-id="feb3a-175">Type</span></span>|<span data-ttu-id="feb3a-176">説明</span><span class="sxs-lookup"><span data-stu-id="feb3a-176">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb3a-177">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="feb3a-177">appliedPolicies</span></span>|<span data-ttu-id="feb3a-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="feb3a-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="feb3a-179">登録済みのアプリが管理サービスと最後に同期したときに、すでに適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="feb3a-179">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="feb3a-180">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-180">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-181">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="feb3a-181">intendedPolicies</span></span>|<span data-ttu-id="feb3a-182">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="feb3a-182">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="feb3a-183">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="feb3a-183">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="feb3a-184">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="feb3a-185">operations</span><span class="sxs-lookup"><span data-stu-id="feb3a-185">operations</span></span>|<span data-ttu-id="feb3a-186">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="feb3a-186">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="feb3a-187">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="feb3a-187">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="feb3a-188">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="feb3a-188">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="feb3a-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="feb3a-189">JSON Representation</span></span>
<span data-ttu-id="feb3a-190">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="feb3a-190">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/appIdentifier:
      Type mismatch between example and table. Parameter name: appIdentifier; example type: (microsoft.graph.androidMobileAppIdentifier); table type: (microsoft.graph.mobileAppIdentifier)",
      "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/flaggedReasons:

      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->
 
