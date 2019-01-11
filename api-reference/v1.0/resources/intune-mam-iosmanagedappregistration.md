---
title: iosManagedAppRegistration リソースの種類
description: 特定のユーザーに対する、iOS アプリの管理機能との同期の詳細を示します。
localization_priority: Normal
ms.openlocfilehash: eb36bf1e96a8b7a54daf9d02b4cc2765a1844d4c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868069"
---
# <a name="iosmanagedappregistration-resource-type"></a><span data-ttu-id="c513c-103">iosManagedAppRegistration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c513c-103">iosManagedAppRegistration resource type</span></span>

> <span data-ttu-id="c513c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c513c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c513c-105">特定のユーザーに対する、iOS アプリの管理機能との同期の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="c513c-105">Represents the synchronization details of an ios app, with management capabilities, for a specific user.</span></span>
<span data-ttu-id="c513c-106">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="c513c-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>

<span data-ttu-id="c513c-107">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-107">Inherits from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c513c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c513c-108">Methods</span></span>
|<span data-ttu-id="c513c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c513c-109">Method</span></span>|<span data-ttu-id="c513c-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c513c-110">Return Type</span></span>|<span data-ttu-id="c513c-111">説明</span><span class="sxs-lookup"><span data-stu-id="c513c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c513c-112">iosManagedAppRegistrations のリスト</span><span class="sxs-lookup"><span data-stu-id="c513c-112">List iosManagedAppRegistrations</span></span>](../api/intune-mam-iosmanagedappregistration-list.md)|<span data-ttu-id="c513c-113">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c513c-113">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) collection</span></span>|<span data-ttu-id="c513c-114">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c513c-114">List properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="c513c-115">iosManagedAppRegistration の取得</span><span class="sxs-lookup"><span data-stu-id="c513c-115">Get iosManagedAppRegistration</span></span>](../api/intune-mam-iosmanagedappregistration-get.md)|[<span data-ttu-id="c513c-116">iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c513c-116">iosManagedAppRegistration</span></span>](../resources/intune-mam-iosmanagedappregistration.md)|<span data-ttu-id="c513c-117">[iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c513c-117">Read properties and relationships of the [iosManagedAppRegistration](../resources/intune-mam-iosmanagedappregistration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c513c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c513c-118">Properties</span></span>
|<span data-ttu-id="c513c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c513c-119">Property</span></span>|<span data-ttu-id="c513c-120">種類</span><span class="sxs-lookup"><span data-stu-id="c513c-120">Type</span></span>|<span data-ttu-id="c513c-121">説明</span><span class="sxs-lookup"><span data-stu-id="c513c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c513c-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c513c-122">createdDateTime</span></span>|<span data-ttu-id="c513c-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c513c-123">DateTimeOffset</span></span>|<span data-ttu-id="c513c-124">作成日時 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="c513c-124">Date and time of creation Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-125">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c513c-125">lastSyncDateTime</span></span>|<span data-ttu-id="c513c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c513c-126">DateTimeOffset</span></span>|<span data-ttu-id="c513c-127">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="c513c-127">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="c513c-128">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-128">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-129">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c513c-129">applicationVersion</span></span>|<span data-ttu-id="c513c-130">String</span><span class="sxs-lookup"><span data-stu-id="c513c-130">String</span></span>|<span data-ttu-id="c513c-131">アプリのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-131">App version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-132">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c513c-132">managementSdkVersion</span></span>|<span data-ttu-id="c513c-133">String</span><span class="sxs-lookup"><span data-stu-id="c513c-133">String</span></span>|<span data-ttu-id="c513c-134">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-134">App management SDK version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-135">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c513c-135">platformVersion</span></span>|<span data-ttu-id="c513c-136">String</span><span class="sxs-lookup"><span data-stu-id="c513c-136">String</span></span>|<span data-ttu-id="c513c-137">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-137">Operating System version Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-138">deviceType</span><span class="sxs-lookup"><span data-stu-id="c513c-138">deviceType</span></span>|<span data-ttu-id="c513c-139">String</span><span class="sxs-lookup"><span data-stu-id="c513c-139">String</span></span>|<span data-ttu-id="c513c-140">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-140">Host device type Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-141">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c513c-141">deviceTag</span></span>|<span data-ttu-id="c513c-142">String</span><span class="sxs-lookup"><span data-stu-id="c513c-142">String</span></span>|<span data-ttu-id="c513c-143">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="c513c-143">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c513c-144">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="c513c-144">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="c513c-145">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-145">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="c513c-146">deviceName</span></span>|<span data-ttu-id="c513c-147">String</span><span class="sxs-lookup"><span data-stu-id="c513c-147">String</span></span>|<span data-ttu-id="c513c-148">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-148">Host device name Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c513c-149">flaggedReasons</span></span>|<span data-ttu-id="c513c-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c513c-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c513c-151">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="c513c-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c513c-152">例:</span><span class="sxs-lookup"><span data-stu-id="c513c-152">E.g.</span></span> <span data-ttu-id="c513c-153">ルートのデバイス上で実行されているアプリ ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-153">app running on rooted device Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-154">userId</span><span class="sxs-lookup"><span data-stu-id="c513c-154">userId</span></span>|<span data-ttu-id="c513c-155">String</span><span class="sxs-lookup"><span data-stu-id="c513c-155">String</span></span>|<span data-ttu-id="c513c-156">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="c513c-156">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="c513c-157">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-157">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-158">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c513c-158">appIdentifier</span></span>|[<span data-ttu-id="c513c-159">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c513c-159">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c513c-160">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="c513c-160">The app package Identifier Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-161">id</span><span class="sxs-lookup"><span data-stu-id="c513c-161">id</span></span>|<span data-ttu-id="c513c-162">String</span><span class="sxs-lookup"><span data-stu-id="c513c-162">String</span></span>|<span data-ttu-id="c513c-163">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c513c-163">Key of the entity.</span></span> <span data-ttu-id="c513c-164">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-164">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-165">version</span><span class="sxs-lookup"><span data-stu-id="c513c-165">version</span></span>|<span data-ttu-id="c513c-166">String</span><span class="sxs-lookup"><span data-stu-id="c513c-166">String</span></span>|<span data-ttu-id="c513c-167">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c513c-167">Version of the entity.</span></span> <span data-ttu-id="c513c-168">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-168">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c513c-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c513c-169">Relationships</span></span>
|<span data-ttu-id="c513c-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c513c-170">Relationship</span></span>|<span data-ttu-id="c513c-171">型</span><span class="sxs-lookup"><span data-stu-id="c513c-171">Type</span></span>|<span data-ttu-id="c513c-172">説明</span><span class="sxs-lookup"><span data-stu-id="c513c-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c513c-173">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c513c-173">appliedPolicies</span></span>|<span data-ttu-id="c513c-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c513c-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c513c-175">登録済みのアプリが管理サービスと最後に同期したときに、すでに適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c513c-175">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span> <span data-ttu-id="c513c-176">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-176">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-177">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="c513c-177">intendedPolicies</span></span>|<span data-ttu-id="c513c-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c513c-178">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c513c-179">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c513c-179">Zero or more policies admin intended for the app as of now.</span></span> <span data-ttu-id="c513c-180">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-180">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|
|<span data-ttu-id="c513c-181">operations</span><span class="sxs-lookup"><span data-stu-id="c513c-181">operations</span></span>|<span data-ttu-id="c513c-182">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c513c-182">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="c513c-183">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="c513c-183">Zero or more long running operations triggered on the app registration.</span></span> <span data-ttu-id="c513c-184">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c513c-184">Inherited from [managedAppRegistration](../resources/intune-mam-managedappregistration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c513c-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c513c-185">JSON Representation</span></span>
<span data-ttu-id="c513c-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c513c-186">Here is a JSON representation of the resource.</span></span>
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
