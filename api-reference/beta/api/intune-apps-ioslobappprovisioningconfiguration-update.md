---
title: Ioslobappプロビジョニング構成の更新
description: Ioslobappプロビジョニング構成オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aee9cde50cfca0c7c4dd0a99047b0b41a7a1639e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33936918"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="a358c-103">Ioslobappプロビジョニング構成の更新</span><span class="sxs-lookup"><span data-stu-id="a358c-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="a358c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a358c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a358c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a358c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a358c-106">[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a358c-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a358c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a358c-107">Prerequisites</span></span>
<span data-ttu-id="a358c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a358c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a358c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a358c-110">Permission type</span></span>|<span data-ttu-id="a358c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a358c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a358c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a358c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a358c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a358c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a358c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a358c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a358c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a358c-115">Not supported.</span></span>|
|<span data-ttu-id="a358c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a358c-116">Application</span></span>|<span data-ttu-id="a358c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a358c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a358c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a358c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a358c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a358c-119">Request headers</span></span>
|<span data-ttu-id="a358c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a358c-120">Header</span></span>|<span data-ttu-id="a358c-121">値</span><span class="sxs-lookup"><span data-stu-id="a358c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a358c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a358c-122">Authorization</span></span>|<span data-ttu-id="a358c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a358c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a358c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a358c-124">Accept</span></span>|<span data-ttu-id="a358c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a358c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a358c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a358c-126">Request body</span></span>
<span data-ttu-id="a358c-127">要求本文で、 [Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a358c-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="a358c-128">次の表に、 [Ioslobapp/構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a358c-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="a358c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a358c-129">Property</span></span>|<span data-ttu-id="a358c-130">型</span><span class="sxs-lookup"><span data-stu-id="a358c-130">Type</span></span>|<span data-ttu-id="a358c-131">説明</span><span class="sxs-lookup"><span data-stu-id="a358c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a358c-132">id</span><span class="sxs-lookup"><span data-stu-id="a358c-132">id</span></span>|<span data-ttu-id="a358c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a358c-133">String</span></span>|<span data-ttu-id="a358c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a358c-134">Key of the entity.</span></span>|
|<span data-ttu-id="a358c-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a358c-135">expirationDateTime</span></span>|<span data-ttu-id="a358c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a358c-136">DateTimeOffset</span></span>|<span data-ttu-id="a358c-137">オプションのプロファイルの有効期限の日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="a358c-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="a358c-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a358c-138">payloadFileName</span></span>|<span data-ttu-id="a358c-139">String</span><span class="sxs-lookup"><span data-stu-id="a358c-139">String</span></span>|<span data-ttu-id="a358c-140">ペイロードファイル名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="a358c-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="a358c-141">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="a358c-141">\*.xml).</span></span>|
|<span data-ttu-id="a358c-142">payload</span><span class="sxs-lookup"><span data-stu-id="a358c-142">payload</span></span>|<span data-ttu-id="a358c-143">Binary</span><span class="sxs-lookup"><span data-stu-id="a358c-143">Binary</span></span>|<span data-ttu-id="a358c-144">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="a358c-144">Payload.</span></span> <span data-ttu-id="a358c-145">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="a358c-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="a358c-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a358c-146">roleScopeTagIds</span></span>|<span data-ttu-id="a358c-147">String collection</span><span class="sxs-lookup"><span data-stu-id="a358c-147">String collection</span></span>|<span data-ttu-id="a358c-148">この iOS LOB アプリプロビジョニング構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a358c-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="a358c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a358c-149">createdDateTime</span></span>|<span data-ttu-id="a358c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a358c-150">DateTimeOffset</span></span>|<span data-ttu-id="a358c-151">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a358c-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="a358c-152">description</span><span class="sxs-lookup"><span data-stu-id="a358c-152">description</span></span>|<span data-ttu-id="a358c-153">String</span><span class="sxs-lookup"><span data-stu-id="a358c-153">String</span></span>|<span data-ttu-id="a358c-154">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="a358c-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="a358c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a358c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="a358c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a358c-156">DateTimeOffset</span></span>|<span data-ttu-id="a358c-157">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a358c-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a358c-158">displayName</span><span class="sxs-lookup"><span data-stu-id="a358c-158">displayName</span></span>|<span data-ttu-id="a358c-159">String</span><span class="sxs-lookup"><span data-stu-id="a358c-159">String</span></span>|<span data-ttu-id="a358c-160">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="a358c-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="a358c-161">version</span><span class="sxs-lookup"><span data-stu-id="a358c-161">version</span></span>|<span data-ttu-id="a358c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="a358c-162">Int32</span></span>|<span data-ttu-id="a358c-163">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a358c-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="a358c-164">応答</span><span class="sxs-lookup"><span data-stu-id="a358c-164">Response</span></span>
<span data-ttu-id="a358c-165">成功した場合、このメソッド`200 OK`は応答コードと、更新された[Ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a358c-165">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a358c-166">例</span><span class="sxs-lookup"><span data-stu-id="a358c-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="a358c-167">要求</span><span class="sxs-lookup"><span data-stu-id="a358c-167">Request</span></span>
<span data-ttu-id="a358c-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a358c-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="a358c-169">応答</span><span class="sxs-lookup"><span data-stu-id="a358c-169">Response</span></span>
<span data-ttu-id="a358c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a358c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 547

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




