---
title: targetedManagedAppConfiguration の作成
description: 新しい targetedManagedAppConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: df5fee37bf26b34367efa9c7f6511de12125f7e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341350"
---
# <a name="create-targetedmanagedappconfiguration"></a><span data-ttu-id="64278-103">targetedManagedAppConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="64278-103">Create targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="64278-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="64278-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64278-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64278-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="64278-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="64278-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64278-107">新しい [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="64278-107">Create a new [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64278-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="64278-108">Prerequisites</span></span>
<span data-ttu-id="64278-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64278-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64278-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64278-111">Permission type</span></span>|<span data-ttu-id="64278-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64278-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64278-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64278-113">Delegated (work or school account)</span></span>|<span data-ttu-id="64278-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64278-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64278-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64278-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64278-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64278-116">Not supported.</span></span>|
|<span data-ttu-id="64278-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64278-117">Application</span></span>|<span data-ttu-id="64278-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64278-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64278-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64278-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64278-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64278-120">Request headers</span></span>
|<span data-ttu-id="64278-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64278-121">Header</span></span>|<span data-ttu-id="64278-122">値</span><span class="sxs-lookup"><span data-stu-id="64278-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64278-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="64278-123">Authorization</span></span>|<span data-ttu-id="64278-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="64278-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64278-125">Accept</span><span class="sxs-lookup"><span data-stu-id="64278-125">Accept</span></span>|<span data-ttu-id="64278-126">application/json</span><span class="sxs-lookup"><span data-stu-id="64278-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64278-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="64278-127">Request body</span></span>
<span data-ttu-id="64278-128">要求本文で、targetedManagedAppConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64278-128">In the request body, supply a JSON representation for the targetedManagedAppConfiguration object.</span></span>

<span data-ttu-id="64278-129">次の表に、targetedManagedAppConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="64278-129">The following table shows the properties that are required when you create the targetedManagedAppConfiguration.</span></span>

|<span data-ttu-id="64278-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64278-130">Property</span></span>|<span data-ttu-id="64278-131">種類</span><span class="sxs-lookup"><span data-stu-id="64278-131">Type</span></span>|<span data-ttu-id="64278-132">説明</span><span class="sxs-lookup"><span data-stu-id="64278-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64278-133">displayName</span><span class="sxs-lookup"><span data-stu-id="64278-133">displayName</span></span>|<span data-ttu-id="64278-134">String</span><span class="sxs-lookup"><span data-stu-id="64278-134">String</span></span>|<span data-ttu-id="64278-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="64278-135">Policy display name.</span></span> <span data-ttu-id="64278-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="64278-137">説明</span><span class="sxs-lookup"><span data-stu-id="64278-137">description</span></span>|<span data-ttu-id="64278-138">String</span><span class="sxs-lookup"><span data-stu-id="64278-138">String</span></span>|<span data-ttu-id="64278-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="64278-139">The policy's description.</span></span> <span data-ttu-id="64278-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="64278-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64278-141">createdDateTime</span></span>|<span data-ttu-id="64278-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64278-142">DateTimeOffset</span></span>|<span data-ttu-id="64278-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="64278-143">The date and time the policy was created.</span></span> <span data-ttu-id="64278-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="64278-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64278-145">lastModifiedDateTime</span></span>|<span data-ttu-id="64278-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64278-146">DateTimeOffset</span></span>|<span data-ttu-id="64278-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="64278-147">Last time the policy was modified.</span></span> <span data-ttu-id="64278-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="64278-149">id</span><span class="sxs-lookup"><span data-stu-id="64278-149">id</span></span>|<span data-ttu-id="64278-150">String</span><span class="sxs-lookup"><span data-stu-id="64278-150">String</span></span>|<span data-ttu-id="64278-151">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="64278-151">Key of the entity.</span></span> <span data-ttu-id="64278-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="64278-153">version</span><span class="sxs-lookup"><span data-stu-id="64278-153">version</span></span>|<span data-ttu-id="64278-154">String</span><span class="sxs-lookup"><span data-stu-id="64278-154">String</span></span>|<span data-ttu-id="64278-155">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="64278-155">Version of the entity.</span></span> <span data-ttu-id="64278-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="64278-157">customSettings</span><span class="sxs-lookup"><span data-stu-id="64278-157">customSettings</span></span>|<span data-ttu-id="64278-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64278-158">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="64278-159">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64278-159">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="64278-160">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="64278-160">deployedAppCount</span></span>|<span data-ttu-id="64278-161">Int32</span><span class="sxs-lookup"><span data-stu-id="64278-161">Int32</span></span>|<span data-ttu-id="64278-162">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="64278-162">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="64278-163">isAssigned</span><span class="sxs-lookup"><span data-stu-id="64278-163">isAssigned</span></span>|<span data-ttu-id="64278-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="64278-164">Boolean</span></span>|<span data-ttu-id="64278-165">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="64278-165">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="64278-166">応答</span><span class="sxs-lookup"><span data-stu-id="64278-166">Response</span></span>
<span data-ttu-id="64278-167">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="64278-167">If successful, this method returns a `201 Created` response code and a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64278-168">例</span><span class="sxs-lookup"><span data-stu-id="64278-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="64278-169">要求</span><span class="sxs-lookup"><span data-stu-id="64278-169">Request</span></span>
<span data-ttu-id="64278-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64278-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
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

### <a name="response"></a><span data-ttu-id="64278-171">応答</span><span class="sxs-lookup"><span data-stu-id="64278-171">Response</span></span>
<span data-ttu-id="64278-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64278-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




