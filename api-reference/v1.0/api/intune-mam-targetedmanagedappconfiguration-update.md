---
title: targetedManagedAppConfiguration の更新
description: targetedManagedAppConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e9cf1f31539789109bc7c538c2a318ae8d685e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916104"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="ff70a-103">targetedManagedAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ff70a-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="ff70a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff70a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff70a-105">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ff70a-105">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff70a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff70a-106">Prerequisites</span></span>
<span data-ttu-id="ff70a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff70a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff70a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff70a-109">Permission type</span></span>|<span data-ttu-id="ff70a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff70a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff70a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff70a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff70a-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff70a-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ff70a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff70a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff70a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff70a-114">Not supported.</span></span>|
|<span data-ttu-id="ff70a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff70a-115">Application</span></span>|<span data-ttu-id="ff70a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff70a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff70a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff70a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ff70a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff70a-118">Request headers</span></span>
|<span data-ttu-id="ff70a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff70a-119">Header</span></span>|<span data-ttu-id="ff70a-120">値</span><span class="sxs-lookup"><span data-stu-id="ff70a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff70a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff70a-121">Authorization</span></span>|<span data-ttu-id="ff70a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ff70a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff70a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ff70a-123">Accept</span></span>|<span data-ttu-id="ff70a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff70a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff70a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff70a-125">Request body</span></span>
<span data-ttu-id="ff70a-126">要求本文で、[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ff70a-126">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="ff70a-127">次の表に、[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ff70a-127">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="ff70a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff70a-128">Property</span></span>|<span data-ttu-id="ff70a-129">型</span><span class="sxs-lookup"><span data-stu-id="ff70a-129">Type</span></span>|<span data-ttu-id="ff70a-130">説明</span><span class="sxs-lookup"><span data-stu-id="ff70a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff70a-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ff70a-131">displayName</span></span>|<span data-ttu-id="ff70a-132">String</span><span class="sxs-lookup"><span data-stu-id="ff70a-132">String</span></span>|<span data-ttu-id="ff70a-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ff70a-133">Policy display name.</span></span> <span data-ttu-id="ff70a-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ff70a-135">説明</span><span class="sxs-lookup"><span data-stu-id="ff70a-135">description</span></span>|<span data-ttu-id="ff70a-136">String</span><span class="sxs-lookup"><span data-stu-id="ff70a-136">String</span></span>|<span data-ttu-id="ff70a-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="ff70a-137">The policy's description.</span></span> <span data-ttu-id="ff70a-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ff70a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ff70a-139">createdDateTime</span></span>|<span data-ttu-id="ff70a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff70a-140">DateTimeOffset</span></span>|<span data-ttu-id="ff70a-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ff70a-141">The date and time the policy was created.</span></span> <span data-ttu-id="ff70a-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ff70a-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff70a-143">lastModifiedDateTime</span></span>|<span data-ttu-id="ff70a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff70a-144">DateTimeOffset</span></span>|<span data-ttu-id="ff70a-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="ff70a-145">Last time the policy was modified.</span></span> <span data-ttu-id="ff70a-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ff70a-147">id</span><span class="sxs-lookup"><span data-stu-id="ff70a-147">id</span></span>|<span data-ttu-id="ff70a-148">String</span><span class="sxs-lookup"><span data-stu-id="ff70a-148">String</span></span>|<span data-ttu-id="ff70a-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ff70a-149">Key of the entity.</span></span> <span data-ttu-id="ff70a-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ff70a-151">version</span><span class="sxs-lookup"><span data-stu-id="ff70a-151">version</span></span>|<span data-ttu-id="ff70a-152">String</span><span class="sxs-lookup"><span data-stu-id="ff70a-152">String</span></span>|<span data-ttu-id="ff70a-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ff70a-153">Version of the entity.</span></span> <span data-ttu-id="ff70a-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ff70a-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="ff70a-155">customSettings</span></span>|<span data-ttu-id="ff70a-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff70a-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="ff70a-157">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ff70a-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="ff70a-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ff70a-158">deployedAppCount</span></span>|<span data-ttu-id="ff70a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="ff70a-159">Int32</span></span>|<span data-ttu-id="ff70a-160">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="ff70a-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ff70a-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ff70a-161">isAssigned</span></span>|<span data-ttu-id="ff70a-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff70a-162">Boolean</span></span>|<span data-ttu-id="ff70a-163">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ff70a-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="ff70a-164">応答</span><span class="sxs-lookup"><span data-stu-id="ff70a-164">Response</span></span>
<span data-ttu-id="ff70a-165">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff70a-165">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff70a-166">例</span><span class="sxs-lookup"><span data-stu-id="ff70a-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff70a-167">要求</span><span class="sxs-lookup"><span data-stu-id="ff70a-167">Request</span></span>
<span data-ttu-id="ff70a-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff70a-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
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

### <a name="response"></a><span data-ttu-id="ff70a-169">応答</span><span class="sxs-lookup"><span data-stu-id="ff70a-169">Response</span></span>
<span data-ttu-id="ff70a-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff70a-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



