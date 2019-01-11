---
title: targetedManagedAppConfiguration の更新
description: targetedManagedAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 77f75233ad54e9d26110640946be7cdab014cb8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813469"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="177c3-103">targetedManagedAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="177c3-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="177c3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="177c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="177c3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="177c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="177c3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="177c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="177c3-107">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="177c3-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="177c3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="177c3-108">Prerequisites</span></span>
<span data-ttu-id="177c3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="177c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="177c3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="177c3-111">Permission type</span></span>|<span data-ttu-id="177c3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="177c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="177c3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="177c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="177c3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="177c3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="177c3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="177c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="177c3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="177c3-116">Not supported.</span></span>|
|<span data-ttu-id="177c3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="177c3-117">Application</span></span>|<span data-ttu-id="177c3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="177c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="177c3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="177c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="177c3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="177c3-120">Request headers</span></span>
|<span data-ttu-id="177c3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="177c3-121">Header</span></span>|<span data-ttu-id="177c3-122">値</span><span class="sxs-lookup"><span data-stu-id="177c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="177c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="177c3-123">Authorization</span></span>|<span data-ttu-id="177c3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="177c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="177c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="177c3-125">Accept</span></span>|<span data-ttu-id="177c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="177c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="177c3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="177c3-127">Request body</span></span>
<span data-ttu-id="177c3-128">要求本文で、[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="177c3-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="177c3-129">次の表に、[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="177c3-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="177c3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="177c3-130">Property</span></span>|<span data-ttu-id="177c3-131">種類</span><span class="sxs-lookup"><span data-stu-id="177c3-131">Type</span></span>|<span data-ttu-id="177c3-132">説明</span><span class="sxs-lookup"><span data-stu-id="177c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="177c3-133">displayName</span><span class="sxs-lookup"><span data-stu-id="177c3-133">displayName</span></span>|<span data-ttu-id="177c3-134">String</span><span class="sxs-lookup"><span data-stu-id="177c3-134">String</span></span>|<span data-ttu-id="177c3-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="177c3-135">Policy display name.</span></span> <span data-ttu-id="177c3-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="177c3-137">説明</span><span class="sxs-lookup"><span data-stu-id="177c3-137">description</span></span>|<span data-ttu-id="177c3-138">String</span><span class="sxs-lookup"><span data-stu-id="177c3-138">String</span></span>|<span data-ttu-id="177c3-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="177c3-139">The policy's description.</span></span> <span data-ttu-id="177c3-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="177c3-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="177c3-141">createdDateTime</span></span>|<span data-ttu-id="177c3-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177c3-142">DateTimeOffset</span></span>|<span data-ttu-id="177c3-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="177c3-143">The date and time the policy was created.</span></span> <span data-ttu-id="177c3-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="177c3-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="177c3-145">lastModifiedDateTime</span></span>|<span data-ttu-id="177c3-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="177c3-146">DateTimeOffset</span></span>|<span data-ttu-id="177c3-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="177c3-147">Last time the policy was modified.</span></span> <span data-ttu-id="177c3-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="177c3-149">id</span><span class="sxs-lookup"><span data-stu-id="177c3-149">id</span></span>|<span data-ttu-id="177c3-150">String</span><span class="sxs-lookup"><span data-stu-id="177c3-150">String</span></span>|<span data-ttu-id="177c3-151">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="177c3-151">Key of the entity.</span></span> <span data-ttu-id="177c3-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="177c3-153">version</span><span class="sxs-lookup"><span data-stu-id="177c3-153">version</span></span>|<span data-ttu-id="177c3-154">String</span><span class="sxs-lookup"><span data-stu-id="177c3-154">String</span></span>|<span data-ttu-id="177c3-155">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="177c3-155">Version of the entity.</span></span> <span data-ttu-id="177c3-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="177c3-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="177c3-157">customSettings</span></span>|<span data-ttu-id="177c3-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="177c3-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="177c3-159">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="177c3-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="177c3-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="177c3-160">deployedAppCount</span></span>|<span data-ttu-id="177c3-161">Int32</span><span class="sxs-lookup"><span data-stu-id="177c3-161">Int32</span></span>|<span data-ttu-id="177c3-162">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="177c3-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="177c3-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="177c3-163">isAssigned</span></span>|<span data-ttu-id="177c3-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="177c3-164">Boolean</span></span>|<span data-ttu-id="177c3-165">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="177c3-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="177c3-166">応答</span><span class="sxs-lookup"><span data-stu-id="177c3-166">Response</span></span>
<span data-ttu-id="177c3-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="177c3-167">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="177c3-168">例</span><span class="sxs-lookup"><span data-stu-id="177c3-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="177c3-169">要求</span><span class="sxs-lookup"><span data-stu-id="177c3-169">Request</span></span>
<span data-ttu-id="177c3-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="177c3-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 382

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="177c3-171">応答</span><span class="sxs-lookup"><span data-stu-id="177c3-171">Response</span></span>
<span data-ttu-id="177c3-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="177c3-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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





