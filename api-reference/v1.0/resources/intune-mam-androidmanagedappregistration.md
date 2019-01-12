---
title: androidManagedAppRegistration リソースの種類
description: 特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 234ee00dd6d2a84720358a889466fd1763e3c80f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970011"
---
# <a name="androidmanagedappregistration-resource-type"></a><span data-ttu-id="ac34f-103">androidManagedAppRegistration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac34f-103">androidManagedAppRegistration resource type</span></span>

> <span data-ttu-id="ac34f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac34f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac34f-105">特定のユーザーに対する、Android アプリの管理機能との同期の詳細を表します。</span><span class="sxs-lookup"><span data-stu-id="ac34f-105">Represents the synchronization details of an android app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="ac34f-106">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="ac34f-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

<span data-ttu-id="ac34f-107">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-107">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ac34f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac34f-108">Methods</span></span>
|<span data-ttu-id="ac34f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="ac34f-109">Method</span></span>|<span data-ttu-id="ac34f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ac34f-110">Return Type</span></span>|<span data-ttu-id="ac34f-111">説明</span><span class="sxs-lookup"><span data-stu-id="ac34f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ac34f-112">androidManagedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="ac34f-112">List androidManagedAppRegistrations</span></span>](../api/intune-mam-androidmanagedappregistration-list.md)|<span data-ttu-id="ac34f-113">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac34f-113">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) collection</span></span>|<span data-ttu-id="ac34f-114">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ac34f-114">List properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="ac34f-115">androidManagedAppRegistration の取得</span><span class="sxs-lookup"><span data-stu-id="ac34f-115">Get androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-get.md)|[<span data-ttu-id="ac34f-116">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ac34f-116">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="ac34f-117">[androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ac34f-117">Read properties and relationships of the [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|
|[<span data-ttu-id="ac34f-118">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="ac34f-118">Create androidManagedAppRegistration</span></span>](../api/intune-mam-androidmanagedappregistration-create.md)|[<span data-ttu-id="ac34f-119">androidManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="ac34f-119">androidManagedAppRegistration</span></span>](../resources/intune-mam-androidmanagedappregistration.md)|<span data-ttu-id="ac34f-120">新しい [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ac34f-120">Create a new [androidManagedAppRegistration](../resources/intune-mam-androidmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ac34f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac34f-121">Properties</span></span>
|<span data-ttu-id="ac34f-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac34f-122">Property</span></span>|<span data-ttu-id="ac34f-123">型</span><span class="sxs-lookup"><span data-stu-id="ac34f-123">Type</span></span>|<span data-ttu-id="ac34f-124">説明</span><span class="sxs-lookup"><span data-stu-id="ac34f-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac34f-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac34f-125">createdDateTime</span></span>|<span data-ttu-id="ac34f-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac34f-126">DateTimeOffset</span></span>|<span data-ttu-id="ac34f-127">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="ac34f-127">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-128">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ac34f-128">lastSyncDateTime</span></span>|<span data-ttu-id="ac34f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac34f-129">DateTimeOffset</span></span>|<span data-ttu-id="ac34f-130">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="ac34f-130">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="ac34f-131">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-131">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-132">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ac34f-132">applicationVersion</span></span>|<span data-ttu-id="ac34f-133">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-133">String</span></span>|<span data-ttu-id="ac34f-134">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-134">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-135">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="ac34f-135">managementSdkVersion</span></span>|<span data-ttu-id="ac34f-136">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-136">String</span></span>|<span data-ttu-id="ac34f-137">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-137">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-138">platformVersion</span><span class="sxs-lookup"><span data-stu-id="ac34f-138">platformVersion</span></span>|<span data-ttu-id="ac34f-139">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-139">String</span></span>|<span data-ttu-id="ac34f-140">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-140">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-141">deviceType</span><span class="sxs-lookup"><span data-stu-id="ac34f-141">deviceType</span></span>|<span data-ttu-id="ac34f-142">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-142">String</span></span>|<span data-ttu-id="ac34f-143">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-143">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-144">deviceTag</span><span class="sxs-lookup"><span data-stu-id="ac34f-144">deviceTag</span></span>|<span data-ttu-id="ac34f-145">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-145">String</span></span>|<span data-ttu-id="ac34f-146">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="ac34f-146">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="ac34f-147">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="ac34f-147">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="ac34f-148">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-148">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="ac34f-149">deviceName</span></span>|<span data-ttu-id="ac34f-150">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-150">String</span></span>|<span data-ttu-id="ac34f-151">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-151">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-152">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="ac34f-152">flaggedReasons</span></span>|<span data-ttu-id="ac34f-153">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ac34f-153">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="ac34f-154">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="ac34f-154">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="ac34f-155">例:</span><span class="sxs-lookup"><span data-stu-id="ac34f-155">E.g.</span></span> <span data-ttu-id="ac34f-156">ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-156">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-157">userId</span><span class="sxs-lookup"><span data-stu-id="ac34f-157">userId</span></span>|<span data-ttu-id="ac34f-158">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-158">String</span></span>|<span data-ttu-id="ac34f-159">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="ac34f-159">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="ac34f-160">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-160">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-161">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac34f-161">appIdentifier</span></span>|[<span data-ttu-id="ac34f-162">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac34f-162">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="ac34f-163">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ac34f-163">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-164">id</span><span class="sxs-lookup"><span data-stu-id="ac34f-164">id</span></span>|<span data-ttu-id="ac34f-165">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-165">String</span></span>|<span data-ttu-id="ac34f-166">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ac34f-166">Key of the entity.</span></span> <span data-ttu-id="ac34f-167">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-167">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-168">version</span><span class="sxs-lookup"><span data-stu-id="ac34f-168">version</span></span>|<span data-ttu-id="ac34f-169">String</span><span class="sxs-lookup"><span data-stu-id="ac34f-169">String</span></span>|<span data-ttu-id="ac34f-170">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ac34f-170">Version of the entity.</span></span> <span data-ttu-id="ac34f-171">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-171">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac34f-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac34f-172">Relationships</span></span>
|<span data-ttu-id="ac34f-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ac34f-173">Relationship</span></span>|<span data-ttu-id="ac34f-174">型</span><span class="sxs-lookup"><span data-stu-id="ac34f-174">Type</span></span>|<span data-ttu-id="ac34f-175">説明</span><span class="sxs-lookup"><span data-stu-id="ac34f-175">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac34f-176">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="ac34f-176">appliedPolicies</span></span>|<span data-ttu-id="ac34f-177">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac34f-177">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="ac34f-178">登録済みのアプリが管理サービスと最後に同期したときに、すでに適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="ac34f-178">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="ac34f-179">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-179">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-180">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="ac34f-180">intendedPolicies</span></span>|<span data-ttu-id="ac34f-181">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac34f-181">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="ac34f-182">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="ac34f-182">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="ac34f-183">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-183">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="ac34f-184">operations</span><span class="sxs-lookup"><span data-stu-id="ac34f-184">operations</span></span>|<span data-ttu-id="ac34f-185">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ac34f-185">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="ac34f-186">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="ac34f-186">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="ac34f-187">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac34f-187">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac34f-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac34f-188">JSON Representation</span></span>
<span data-ttu-id="ac34f-189">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac34f-189">Here is a JSON representation of the resource.</span></span>
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
    "@odata.type": "microsoft.graph.mobileAppIdentifier",
    "packageId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-androidmanagedappregistration.md/microsoft.graph.androidManagedAppRegistration/flaggedReasons:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->



