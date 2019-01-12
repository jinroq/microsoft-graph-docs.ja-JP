---
title: managedAppRegistration リソース タイプ
description: ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8a954c3465ba4bb4d2f7372ee544a00fcd8c2af7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937090"
---
# <a name="managedappregistration-resource-type"></a><span data-ttu-id="c86ce-103">managedAppRegistration リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c86ce-103">managedAppRegistration resource type</span></span>

> <span data-ttu-id="c86ce-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c86ce-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c86ce-105">ManagedAppEntity は、アプリ管理ワークフロー下にある他のすべてのエンティティ タイプの基本型です。</span><span class="sxs-lookup"><span data-stu-id="c86ce-105">The ManagedAppEntity is the base entity type for all other entity types under app management workflow.</span></span>
<span data-ttu-id="c86ce-106">ManagedAppRegistration リソースは、組織のメンバーに使用されるアプリの詳細を管理機能と共に示します。</span><span class="sxs-lookup"><span data-stu-id="c86ce-106">The ManagedAppRegistration resource represents the details of an app, with management capability, used by a member of the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="c86ce-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c86ce-107">Methods</span></span>
|<span data-ttu-id="c86ce-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c86ce-108">Method</span></span>|<span data-ttu-id="c86ce-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c86ce-109">Return Type</span></span>|<span data-ttu-id="c86ce-110">説明</span><span class="sxs-lookup"><span data-stu-id="c86ce-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c86ce-111">List managedAppRegistrations</span><span class="sxs-lookup"><span data-stu-id="c86ce-111">List managedAppRegistrations</span></span>](../api/intune-mam-managedappregistration-list.md)|<span data-ttu-id="c86ce-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c86ce-112">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) collection</span></span>|<span data-ttu-id="c86ce-113">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c86ce-113">List properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) objects.</span></span>|
|[<span data-ttu-id="c86ce-114">Get managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c86ce-114">Get managedAppRegistration</span></span>](../api/intune-mam-managedappregistration-get.md)|[<span data-ttu-id="c86ce-115">managedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="c86ce-115">managedAppRegistration</span></span>](../resources/intune-mam-managedappregistration.md)|<span data-ttu-id="c86ce-116">[managedAppRegistration](../resources/intune-mam-managedappregistration.md) オブジェクトのプロパティとリレーションを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c86ce-116">Read properties and relationships of the [managedAppRegistration](../resources/intune-mam-managedappregistration.md) object.</span></span>|
|[<span data-ttu-id="c86ce-117">getUserIdsWithFlaggedAppRegistration function</span><span class="sxs-lookup"><span data-stu-id="c86ce-117">getUserIdsWithFlaggedAppRegistration function</span></span>](../api/intune-mam-managedappregistration-getuseridswithflaggedappregistration.md)|<span data-ttu-id="c86ce-118">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c86ce-118">String collection</span></span>|<span data-ttu-id="c86ce-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c86ce-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c86ce-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c86ce-120">Properties</span></span>
|<span data-ttu-id="c86ce-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c86ce-121">Property</span></span>|<span data-ttu-id="c86ce-122">種類</span><span class="sxs-lookup"><span data-stu-id="c86ce-122">Type</span></span>|<span data-ttu-id="c86ce-123">説明</span><span class="sxs-lookup"><span data-stu-id="c86ce-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c86ce-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c86ce-124">createdDateTime</span></span>|<span data-ttu-id="c86ce-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c86ce-125">DateTimeOffset</span></span>|<span data-ttu-id="c86ce-126">作成日時</span><span class="sxs-lookup"><span data-stu-id="c86ce-126">Date and time of creation</span></span>|
|<span data-ttu-id="c86ce-127">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="c86ce-127">lastSyncDateTime</span></span>|<span data-ttu-id="c86ce-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c86ce-128">DateTimeOffset</span></span>|<span data-ttu-id="c86ce-129">アプリが管理サービスと最後に同期した日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c86ce-129">Date and time of last the app synced with management service.</span></span>|
|<span data-ttu-id="c86ce-130">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="c86ce-130">applicationVersion</span></span>|<span data-ttu-id="c86ce-131">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-131">String</span></span>|<span data-ttu-id="c86ce-132">アプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="c86ce-132">App version</span></span>|
|<span data-ttu-id="c86ce-133">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="c86ce-133">managementSdkVersion</span></span>|<span data-ttu-id="c86ce-134">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-134">String</span></span>|<span data-ttu-id="c86ce-135">アプリ管理の SDK バージョン</span><span class="sxs-lookup"><span data-stu-id="c86ce-135">App management SDK version</span></span>|
|<span data-ttu-id="c86ce-136">platformVersion</span><span class="sxs-lookup"><span data-stu-id="c86ce-136">platformVersion</span></span>|<span data-ttu-id="c86ce-137">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-137">String</span></span>|<span data-ttu-id="c86ce-138">オペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="c86ce-138">Operating System version</span></span>|
|<span data-ttu-id="c86ce-139">deviceType</span><span class="sxs-lookup"><span data-stu-id="c86ce-139">deviceType</span></span>|<span data-ttu-id="c86ce-140">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-140">String</span></span>|<span data-ttu-id="c86ce-141">ホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="c86ce-141">Host device type</span></span>|
|<span data-ttu-id="c86ce-142">deviceTag</span><span class="sxs-lookup"><span data-stu-id="c86ce-142">deviceTag</span></span>|<span data-ttu-id="c86ce-143">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-143">String</span></span>|<span data-ttu-id="c86ce-144">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="c86ce-144">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="c86ce-145">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="c86ce-145">Not guaranteed to relate apps in all conditions.</span></span>|
|<span data-ttu-id="c86ce-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="c86ce-146">deviceName</span></span>|<span data-ttu-id="c86ce-147">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-147">String</span></span>|<span data-ttu-id="c86ce-148">ホスト デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="c86ce-148">Host device name</span></span>|
|<span data-ttu-id="c86ce-149">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="c86ce-149">flaggedReasons</span></span>|<span data-ttu-id="c86ce-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c86ce-150">[managedAppFlaggedReason](../resources/intune-mam-managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="c86ce-151">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="c86ce-151">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="c86ce-152">例:</span><span class="sxs-lookup"><span data-stu-id="c86ce-152">E.g.</span></span> <span data-ttu-id="c86ce-153">ルートのデバイスで実行されているアプリ</span><span class="sxs-lookup"><span data-stu-id="c86ce-153">app running on rooted device</span></span>|
|<span data-ttu-id="c86ce-154">userId</span><span class="sxs-lookup"><span data-stu-id="c86ce-154">userId</span></span>|<span data-ttu-id="c86ce-155">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-155">String</span></span>|<span data-ttu-id="c86ce-156">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="c86ce-156">The user Id to who this app registration belongs.</span></span>|
|<span data-ttu-id="c86ce-157">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="c86ce-157">appIdentifier</span></span>|[<span data-ttu-id="c86ce-158">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="c86ce-158">mobileAppIdentifier</span></span>](../resources/intune-mam-mobileappidentifier.md)|<span data-ttu-id="c86ce-159">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="c86ce-159">The app package Identifier</span></span>|
|<span data-ttu-id="c86ce-160">id</span><span class="sxs-lookup"><span data-stu-id="c86ce-160">id</span></span>|<span data-ttu-id="c86ce-161">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-161">String</span></span>|<span data-ttu-id="c86ce-162">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c86ce-162">Key of the entity.</span></span>|
|<span data-ttu-id="c86ce-163">version</span><span class="sxs-lookup"><span data-stu-id="c86ce-163">version</span></span>|<span data-ttu-id="c86ce-164">String</span><span class="sxs-lookup"><span data-stu-id="c86ce-164">String</span></span>|<span data-ttu-id="c86ce-165">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c86ce-165">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c86ce-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c86ce-166">Relationships</span></span>
|<span data-ttu-id="c86ce-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c86ce-167">Relationship</span></span>|<span data-ttu-id="c86ce-168">型</span><span class="sxs-lookup"><span data-stu-id="c86ce-168">Type</span></span>|<span data-ttu-id="c86ce-169">説明</span><span class="sxs-lookup"><span data-stu-id="c86ce-169">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c86ce-170">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="c86ce-170">appliedPolicies</span></span>|<span data-ttu-id="c86ce-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c86ce-171">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c86ce-172">登録済みのアプリが管理サービスと最後に同期したときに、既に適用されていた 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c86ce-172">Zero or more policys already applied on the registered app when it last synchronized with managment service.</span></span>|
|<span data-ttu-id="c86ce-173">intendedPolicies</span><span class="sxs-lookup"><span data-stu-id="c86ce-173">intendedPolicies</span></span>|<span data-ttu-id="c86ce-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c86ce-174">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection</span></span>|<span data-ttu-id="c86ce-175">現時点で、管理者がアプリに対して意図した 0 個以上のポリシーです。</span><span class="sxs-lookup"><span data-stu-id="c86ce-175">Zero or more policies admin intended for the app as of now.</span></span>|
|<span data-ttu-id="c86ce-176">operations</span><span class="sxs-lookup"><span data-stu-id="c86ce-176">operations</span></span>|<span data-ttu-id="c86ce-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c86ce-177">[managedAppOperation](../resources/intune-mam-managedappoperation.md) collection</span></span>|<span data-ttu-id="c86ce-178">アプリ登録でトリガーされた、0 個以上の長時間実行の操作です。</span><span class="sxs-lookup"><span data-stu-id="c86ce-178">Zero or more long running operations triggered on the app registration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c86ce-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c86ce-179">JSON Representation</span></span>
<span data-ttu-id="c86ce-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c86ce-180">Here is a JSON representation of the resource.</span></span>
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
