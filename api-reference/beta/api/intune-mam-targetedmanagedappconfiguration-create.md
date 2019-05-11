---
title: targetedManagedAppConfiguration の作成
description: 新しい targetedManagedAppConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ccb8e9e9e9c592759b73aa022d0a21ceb61fc785
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33903068"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="351ac-103">targetedManagedAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="351ac-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="351ac-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="351ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="351ac-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="351ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="351ac-106">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="351ac-106">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="351ac-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="351ac-107">Prerequisites</span></span>
<span data-ttu-id="351ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="351ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="351ac-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="351ac-110">Permission type</span></span>|<span data-ttu-id="351ac-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="351ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="351ac-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="351ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="351ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="351ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="351ac-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="351ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="351ac-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="351ac-115">Not supported.</span></span>|
|<span data-ttu-id="351ac-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="351ac-116">Application</span></span>|<span data-ttu-id="351ac-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="351ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="351ac-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="351ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="351ac-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="351ac-119">Request headers</span></span>
|<span data-ttu-id="351ac-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="351ac-120">Header</span></span>|<span data-ttu-id="351ac-121">値</span><span class="sxs-lookup"><span data-stu-id="351ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="351ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="351ac-122">Authorization</span></span>|<span data-ttu-id="351ac-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="351ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="351ac-124">承諾</span><span class="sxs-lookup"><span data-stu-id="351ac-124">Accept</span></span>|<span data-ttu-id="351ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="351ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="351ac-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="351ac-126">Request body</span></span>
<span data-ttu-id="351ac-127">要求本文で、targetedManagedAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="351ac-127">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="351ac-128">次の表に、targetedManagedAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="351ac-128">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="351ac-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="351ac-129">Property</span></span>|<span data-ttu-id="351ac-130">型</span><span class="sxs-lookup"><span data-stu-id="351ac-130">Type</span></span>|<span data-ttu-id="351ac-131">説明</span><span class="sxs-lookup"><span data-stu-id="351ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="351ac-132">displayName</span><span class="sxs-lookup"><span data-stu-id="351ac-132">displayName</span></span>|<span data-ttu-id="351ac-133">String</span><span class="sxs-lookup"><span data-stu-id="351ac-133">String</span></span>|<span data-ttu-id="351ac-134">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="351ac-134">Policy display name.</span></span> <span data-ttu-id="351ac-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-136">description</span><span class="sxs-lookup"><span data-stu-id="351ac-136">description</span></span>|<span data-ttu-id="351ac-137">String</span><span class="sxs-lookup"><span data-stu-id="351ac-137">String</span></span>|<span data-ttu-id="351ac-138">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="351ac-138">The policy's description.</span></span> <span data-ttu-id="351ac-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="351ac-140">createdDateTime</span></span>|<span data-ttu-id="351ac-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="351ac-141">DateTimeOffset</span></span>|<span data-ttu-id="351ac-142">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="351ac-142">The date and time the policy was created.</span></span> <span data-ttu-id="351ac-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="351ac-144">lastModifiedDateTime</span></span>|<span data-ttu-id="351ac-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="351ac-145">DateTimeOffset</span></span>|<span data-ttu-id="351ac-146">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="351ac-146">Last time the policy was modified.</span></span> <span data-ttu-id="351ac-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="351ac-148">roleScopeTagIds</span></span>|<span data-ttu-id="351ac-149">String collection</span><span class="sxs-lookup"><span data-stu-id="351ac-149">String collection</span></span>|<span data-ttu-id="351ac-150">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="351ac-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="351ac-151">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-152">id</span><span class="sxs-lookup"><span data-stu-id="351ac-152">id</span></span>|<span data-ttu-id="351ac-153">文字列</span><span class="sxs-lookup"><span data-stu-id="351ac-153">String</span></span>|<span data-ttu-id="351ac-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="351ac-154">Key of the entity.</span></span> <span data-ttu-id="351ac-155">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-156">version</span><span class="sxs-lookup"><span data-stu-id="351ac-156">version</span></span>|<span data-ttu-id="351ac-157">String</span><span class="sxs-lookup"><span data-stu-id="351ac-157">String</span></span>|<span data-ttu-id="351ac-158">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="351ac-158">Version of the entity.</span></span> <span data-ttu-id="351ac-159">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="351ac-160">customSettings</span><span class="sxs-lookup"><span data-stu-id="351ac-160">customSettings</span></span>|<span data-ttu-id="351ac-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="351ac-161">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="351ac-162">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="351ac-162">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="351ac-163">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="351ac-163">deployedAppCount</span></span>|<span data-ttu-id="351ac-164">Int32</span><span class="sxs-lookup"><span data-stu-id="351ac-164">Int32</span></span>|<span data-ttu-id="351ac-165">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="351ac-165">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="351ac-166">isAssigned</span><span class="sxs-lookup"><span data-stu-id="351ac-166">isAssigned</span></span>|<span data-ttu-id="351ac-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="351ac-167">Boolean</span></span>|<span data-ttu-id="351ac-168">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="351ac-168">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="351ac-169">応答</span><span class="sxs-lookup"><span data-stu-id="351ac-169">Response</span></span>
<span data-ttu-id="351ac-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="351ac-170">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="351ac-171">例</span><span class="sxs-lookup"><span data-stu-id="351ac-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="351ac-172">要求</span><span class="sxs-lookup"><span data-stu-id="351ac-172">Request</span></span>
<span data-ttu-id="351ac-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="351ac-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 450

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="351ac-174">応答</span><span class="sxs-lookup"><span data-stu-id="351ac-174">Response</span></span>
<span data-ttu-id="351ac-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="351ac-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```




