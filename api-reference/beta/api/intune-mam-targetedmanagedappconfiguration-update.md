---
title: targetedManagedAppConfiguration の更新
description: targetedManagedAppConfiguration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eded21015054073b6f6711faecd5c01da52fece0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403694"
---
# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="04200-103">targetedManagedAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="04200-103">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="04200-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04200-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04200-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04200-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04200-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04200-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04200-107">[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="04200-107">Update the properties of a [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04200-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="04200-108">Prerequisites</span></span>
<span data-ttu-id="04200-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04200-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04200-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04200-111">Permission type</span></span>|<span data-ttu-id="04200-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04200-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04200-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04200-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04200-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04200-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="04200-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04200-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04200-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04200-116">Not supported.</span></span>|
|<span data-ttu-id="04200-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04200-117">Application</span></span>|<span data-ttu-id="04200-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04200-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04200-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04200-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="04200-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04200-120">Request headers</span></span>
|<span data-ttu-id="04200-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04200-121">Header</span></span>|<span data-ttu-id="04200-122">値</span><span class="sxs-lookup"><span data-stu-id="04200-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04200-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04200-123">Authorization</span></span>|<span data-ttu-id="04200-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="04200-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04200-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04200-125">Accept</span></span>|<span data-ttu-id="04200-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04200-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04200-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04200-127">Request body</span></span>
<span data-ttu-id="04200-128">要求本文で、[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="04200-128">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="04200-129">次の表に、[targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="04200-129">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="04200-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04200-130">Property</span></span>|<span data-ttu-id="04200-131">型</span><span class="sxs-lookup"><span data-stu-id="04200-131">Type</span></span>|<span data-ttu-id="04200-132">説明</span><span class="sxs-lookup"><span data-stu-id="04200-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04200-133">displayName</span><span class="sxs-lookup"><span data-stu-id="04200-133">displayName</span></span>|<span data-ttu-id="04200-134">String</span><span class="sxs-lookup"><span data-stu-id="04200-134">String</span></span>|<span data-ttu-id="04200-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="04200-135">Policy display name.</span></span> <span data-ttu-id="04200-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-137">説明</span><span class="sxs-lookup"><span data-stu-id="04200-137">description</span></span>|<span data-ttu-id="04200-138">String</span><span class="sxs-lookup"><span data-stu-id="04200-138">String</span></span>|<span data-ttu-id="04200-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="04200-139">The policy's description.</span></span> <span data-ttu-id="04200-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04200-141">createdDateTime</span></span>|<span data-ttu-id="04200-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04200-142">DateTimeOffset</span></span>|<span data-ttu-id="04200-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="04200-143">The date and time the policy was created.</span></span> <span data-ttu-id="04200-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04200-145">lastModifiedDateTime</span></span>|<span data-ttu-id="04200-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04200-146">DateTimeOffset</span></span>|<span data-ttu-id="04200-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="04200-147">Last time the policy was modified.</span></span> <span data-ttu-id="04200-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04200-149">roleScopeTagIds</span></span>|<span data-ttu-id="04200-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="04200-150">String collection</span></span>|<span data-ttu-id="04200-151">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="04200-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="04200-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-153">id</span><span class="sxs-lookup"><span data-stu-id="04200-153">id</span></span>|<span data-ttu-id="04200-154">String</span><span class="sxs-lookup"><span data-stu-id="04200-154">String</span></span>|<span data-ttu-id="04200-155">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04200-155">Key of the entity.</span></span> <span data-ttu-id="04200-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-157">version</span><span class="sxs-lookup"><span data-stu-id="04200-157">version</span></span>|<span data-ttu-id="04200-158">String</span><span class="sxs-lookup"><span data-stu-id="04200-158">String</span></span>|<span data-ttu-id="04200-159">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="04200-159">Version of the entity.</span></span> <span data-ttu-id="04200-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="04200-161">customSettings</span><span class="sxs-lookup"><span data-stu-id="04200-161">customSettings</span></span>|<span data-ttu-id="04200-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="04200-162">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="04200-163">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04200-163">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md)</span></span>|
|<span data-ttu-id="04200-164">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="04200-164">deployedAppCount</span></span>|<span data-ttu-id="04200-165">Int32</span><span class="sxs-lookup"><span data-stu-id="04200-165">Int32</span></span>|<span data-ttu-id="04200-166">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="04200-166">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="04200-167">isAssigned</span><span class="sxs-lookup"><span data-stu-id="04200-167">isAssigned</span></span>|<span data-ttu-id="04200-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="04200-168">Boolean</span></span>|<span data-ttu-id="04200-169">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="04200-169">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="04200-170">応答</span><span class="sxs-lookup"><span data-stu-id="04200-170">Response</span></span>
<span data-ttu-id="04200-171">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="04200-171">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune-mam-targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04200-172">例</span><span class="sxs-lookup"><span data-stu-id="04200-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="04200-173">要求</span><span class="sxs-lookup"><span data-stu-id="04200-173">Request</span></span>
<span data-ttu-id="04200-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04200-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
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

### <a name="response"></a><span data-ttu-id="04200-175">応答</span><span class="sxs-lookup"><span data-stu-id="04200-175">Response</span></span>
<span data-ttu-id="04200-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04200-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




