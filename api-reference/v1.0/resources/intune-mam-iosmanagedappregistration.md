---
title: iosManagedAppRegistration リソースの種類
description: 特定のユーザーに対する、iOS アプリの管理機能との同期の詳細を示します。 ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29c8798898ea4e3e95ee051348363e0e0ba0ff71
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465490"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="2ac19-104">iosManagedAppRegistration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ac19-104">iosManagedAppRegistration resource type</span></span>

> <span data-ttu-id="2ac19-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2ac19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ac19-106">特定のユーザーに対する、iOS アプリの管理機能との同期の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="2ac19-106">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="2ac19-107">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="2ac19-107">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>


<span data-ttu-id="2ac19-108">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-108">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2ac19-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ac19-109">Methods</span></span>
|<span data-ttu-id="2ac19-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="2ac19-110">Method</span></span>|<span data-ttu-id="2ac19-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2ac19-111">Return Type</span></span>|<span data-ttu-id="2ac19-112">説明</span><span class="sxs-lookup"><span data-stu-id="2ac19-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2ac19-113">iosManagedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="2ac19-113">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="2ac19-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ac19-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="2ac19-115">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2ac19-115">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="2ac19-116">iosManagedAppRegistration の取得</span><span class="sxs-lookup"><span data-stu-id="2ac19-116">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="2ac19-117">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="2ac19-117">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="2ac19-118">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2ac19-118">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2ac19-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ac19-119">Properties</span></span>
|<span data-ttu-id="2ac19-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ac19-120">Property</span></span>|<span data-ttu-id="2ac19-121">型</span><span class="sxs-lookup"><span data-stu-id="2ac19-121">Type</span></span>|<span data-ttu-id="2ac19-122">説明</span><span class="sxs-lookup"><span data-stu-id="2ac19-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac19-123">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac19-123">createdDateTime</span></span>|<span data-ttu-id="2ac19-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac19-124">DateTimeOffset</span></span>|<span data-ttu-id="2ac19-125">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="2ac19-125">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-126">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2ac19-126">lastSyncDateTime</span></span>|<span data-ttu-id="2ac19-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ac19-127">DateTimeOffset</span></span>|<span data-ttu-id="2ac19-128">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="2ac19-128">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="2ac19-129">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-129">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="2ac19-130">applicationVersion</span></span>|<span data-ttu-id="2ac19-131">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-131">String</span></span>|<span data-ttu-id="2ac19-132">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-132">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="2ac19-133">managementSdkVersion</span></span>|<span data-ttu-id="2ac19-134">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-134">String</span></span>|<span data-ttu-id="2ac19-135">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-135">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="2ac19-136">platformVersion</span></span>|<span data-ttu-id="2ac19-137">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-137">String</span></span>|<span data-ttu-id="2ac19-138">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-138">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="2ac19-139">deviceType</span></span>|<span data-ttu-id="2ac19-140">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-140">String</span></span>|<span data-ttu-id="2ac19-141">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-141">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="2ac19-142">deviceTag</span></span>|<span data-ttu-id="2ac19-143">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-143">String</span></span>|<span data-ttu-id="2ac19-144">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="2ac19-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="2ac19-145">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="2ac19-145">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="2ac19-146">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-146">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="2ac19-147">deviceName</span></span>|<span data-ttu-id="2ac19-148">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-148">String</span></span>|<span data-ttu-id="2ac19-149">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-149">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-150">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="2ac19-150">flaggedReasons</span></span>|<span data-ttu-id="2ac19-151">[managedappflaggedreason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2ac19-151">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="2ac19-152">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="2ac19-152">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="2ac19-153">例:</span><span class="sxs-lookup"><span data-stu-id="2ac19-153">E.g.</span></span> <span data-ttu-id="2ac19-154">ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-154">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-155">userId</span><span class="sxs-lookup"><span data-stu-id="2ac19-155">userId</span></span>|<span data-ttu-id="2ac19-156">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-156">String</span></span>|<span data-ttu-id="2ac19-157">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="2ac19-157">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="2ac19-158">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-158">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-159">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ac19-159">appIdentifier</span></span>|[<span data-ttu-id="2ac19-160">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ac19-160">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="2ac19-161">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="2ac19-161">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-162">id</span><span class="sxs-lookup"><span data-stu-id="2ac19-162">id</span></span>|<span data-ttu-id="2ac19-163">String</span><span class="sxs-lookup"><span data-stu-id="2ac19-163">String</span></span>|<span data-ttu-id="2ac19-164">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2ac19-164">Key of the entity.</span></span> <span data-ttu-id="2ac19-165">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-165">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-166">version</span><span class="sxs-lookup"><span data-stu-id="2ac19-166">version</span></span>|<span data-ttu-id="2ac19-167">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2ac19-167">String</span></span>|<span data-ttu-id="2ac19-168">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2ac19-168">Version of the entity.</span></span> <span data-ttu-id="2ac19-169">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-169">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ac19-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ac19-170">Relationships</span></span>
|<span data-ttu-id="2ac19-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ac19-171">Relationship</span></span>|<span data-ttu-id="2ac19-172">型</span><span class="sxs-lookup"><span data-stu-id="2ac19-172">Type</span></span>|<span data-ttu-id="2ac19-173">説明</span><span class="sxs-lookup"><span data-stu-id="2ac19-173">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ac19-174">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="2ac19-174">appliedPolicies</span></span>|<span data-ttu-id="2ac19-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ac19-175">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2ac19-176">登録済みのアプリが管理サービスと最後に同期したときに、すでに適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="2ac19-176">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="2ac19-177">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-177">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-178">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="2ac19-178">intendedPolicies</span></span>|<span data-ttu-id="2ac19-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ac19-179">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="2ac19-180">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="2ac19-180">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="2ac19-181">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-181">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="2ac19-182">operations</span><span class="sxs-lookup"><span data-stu-id="2ac19-182">operations</span></span>|<span data-ttu-id="2ac19-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2ac19-183">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="2ac19-184">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="2ac19-184">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="2ac19-185">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2ac19-185">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2ac19-186">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ac19-186">JSON Representation</span></span>
<span data-ttu-id="2ac19-187">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2ac19-187">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppRegistration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
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
    "bundleId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-iosmanagedappregistration.md/microsoft.graph.iosManagedAppRegistration/flaggedReasons:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->

