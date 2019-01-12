---
title: targetedManagedAppConfiguration の作成
description: 新しい targetedManagedAppConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc7175a3ad6f43393e52de2c55a2dc6cbc7bea65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934724"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="a080f-103">targetedManagedAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a080f-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="a080f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a080f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a080f-105">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a080f-105">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a080f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a080f-106">Prerequisites</span></span>
<span data-ttu-id="a080f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a080f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a080f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a080f-109">Permission type</span></span>|<span data-ttu-id="a080f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a080f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a080f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a080f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a080f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a080f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a080f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a080f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a080f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a080f-114">Not supported.</span></span>|
|<span data-ttu-id="a080f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a080f-115">Application</span></span>|<span data-ttu-id="a080f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a080f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a080f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a080f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a080f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a080f-118">Request headers</span></span>
|<span data-ttu-id="a080f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a080f-119">Header</span></span>|<span data-ttu-id="a080f-120">値</span><span class="sxs-lookup"><span data-stu-id="a080f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a080f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a080f-121">Authorization</span></span>|<span data-ttu-id="a080f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a080f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a080f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a080f-123">Accept</span></span>|<span data-ttu-id="a080f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a080f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a080f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a080f-125">Request body</span></span>
<span data-ttu-id="a080f-126">要求本文で、targetedManagedAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a080f-126">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="a080f-127">次の表に、targetedManagedAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a080f-127">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="a080f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a080f-128">Property</span></span>|<span data-ttu-id="a080f-129">型</span><span class="sxs-lookup"><span data-stu-id="a080f-129">Type</span></span>|<span data-ttu-id="a080f-130">説明</span><span class="sxs-lookup"><span data-stu-id="a080f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a080f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="a080f-131">displayName</span></span>|<span data-ttu-id="a080f-132">String</span><span class="sxs-lookup"><span data-stu-id="a080f-132">String</span></span>|<span data-ttu-id="a080f-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="a080f-133">Policy display name.</span></span> <span data-ttu-id="a080f-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a080f-135">説明</span><span class="sxs-lookup"><span data-stu-id="a080f-135">description</span></span>|<span data-ttu-id="a080f-136">String</span><span class="sxs-lookup"><span data-stu-id="a080f-136">String</span></span>|<span data-ttu-id="a080f-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="a080f-137">The policy's description.</span></span> <span data-ttu-id="a080f-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a080f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a080f-139">createdDateTime</span></span>|<span data-ttu-id="a080f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a080f-140">DateTimeOffset</span></span>|<span data-ttu-id="a080f-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a080f-141">The date and time the policy was created.</span></span> <span data-ttu-id="a080f-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a080f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a080f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="a080f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a080f-144">DateTimeOffset</span></span>|<span data-ttu-id="a080f-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="a080f-145">Last time the policy was modified.</span></span> <span data-ttu-id="a080f-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a080f-147">id</span><span class="sxs-lookup"><span data-stu-id="a080f-147">id</span></span>|<span data-ttu-id="a080f-148">String</span><span class="sxs-lookup"><span data-stu-id="a080f-148">String</span></span>|<span data-ttu-id="a080f-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a080f-149">Key of the entity.</span></span> <span data-ttu-id="a080f-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a080f-151">version</span><span class="sxs-lookup"><span data-stu-id="a080f-151">version</span></span>|<span data-ttu-id="a080f-152">String</span><span class="sxs-lookup"><span data-stu-id="a080f-152">String</span></span>|<span data-ttu-id="a080f-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="a080f-153">Version of the entity.</span></span> <span data-ttu-id="a080f-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="a080f-155">customSettings</span><span class="sxs-lookup"><span data-stu-id="a080f-155">customSettings</span></span>|<span data-ttu-id="a080f-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a080f-156">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="a080f-157">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a080f-157">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="a080f-158">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="a080f-158">deployedAppCount</span></span>|<span data-ttu-id="a080f-159">Int32</span><span class="sxs-lookup"><span data-stu-id="a080f-159">Int32</span></span>|<span data-ttu-id="a080f-160">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="a080f-160">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="a080f-161">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a080f-161">isAssigned</span></span>|<span data-ttu-id="a080f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a080f-162">Boolean</span></span>|<span data-ttu-id="a080f-163">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a080f-163">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="a080f-164">応答</span><span class="sxs-lookup"><span data-stu-id="a080f-164">Response</span></span>
<span data-ttu-id="a080f-165">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a080f-165">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a080f-166">例</span><span class="sxs-lookup"><span data-stu-id="a080f-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="a080f-167">要求</span><span class="sxs-lookup"><span data-stu-id="a080f-167">Request</span></span>
<span data-ttu-id="a080f-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a080f-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations
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

### <a name="response"></a><span data-ttu-id="a080f-169">応答</span><span class="sxs-lookup"><span data-stu-id="a080f-169">Response</span></span>
<span data-ttu-id="a080f-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a080f-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



