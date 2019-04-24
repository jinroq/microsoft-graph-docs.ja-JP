---
title: ioslobappプロビジョニング構成の更新
description: ioslobappプロビジョニング構成オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ff8d2bc9bc92be592bee5fdf9c03255d08d1a21
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32496101"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="c3ff3-103">ioslobappプロビジョニング構成の更新</span><span class="sxs-lookup"><span data-stu-id="c3ff3-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="c3ff3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3ff3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ff3-106">[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3ff3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3ff3-107">Prerequisites</span></span>
<span data-ttu-id="c3ff3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3ff3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3ff3-110">Permission type</span></span>|<span data-ttu-id="c3ff3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3ff3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3ff3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3ff3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3ff3-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3ff3-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3ff3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3ff3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3ff3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-115">Not supported.</span></span>|
|<span data-ttu-id="c3ff3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3ff3-116">Application</span></span>|<span data-ttu-id="c3ff3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3ff3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3ff3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c3ff3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3ff3-119">Request headers</span></span>
|<span data-ttu-id="c3ff3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3ff3-120">Header</span></span>|<span data-ttu-id="c3ff3-121">値</span><span class="sxs-lookup"><span data-stu-id="c3ff3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3ff3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3ff3-122">Authorization</span></span>|<span data-ttu-id="c3ff3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3ff3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c3ff3-124">Accept</span></span>|<span data-ttu-id="c3ff3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3ff3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3ff3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3ff3-126">Request body</span></span>
<span data-ttu-id="c3ff3-127">要求本文で、 [ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="c3ff3-128">次の表に、 [ioslobapp/構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="c3ff3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3ff3-129">Property</span></span>|<span data-ttu-id="c3ff3-130">型</span><span class="sxs-lookup"><span data-stu-id="c3ff3-130">Type</span></span>|<span data-ttu-id="c3ff3-131">説明</span><span class="sxs-lookup"><span data-stu-id="c3ff3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ff3-132">id</span><span class="sxs-lookup"><span data-stu-id="c3ff3-132">id</span></span>|<span data-ttu-id="c3ff3-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c3ff3-133">String</span></span>|<span data-ttu-id="c3ff3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-134">Key of the entity.</span></span>|
|<span data-ttu-id="c3ff3-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c3ff3-135">expirationDateTime</span></span>|<span data-ttu-id="c3ff3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3ff3-136">DateTimeOffset</span></span>|<span data-ttu-id="c3ff3-137">オプションのプロファイルの有効期限の日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="c3ff3-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c3ff3-138">payloadFileName</span></span>|<span data-ttu-id="c3ff3-139">String</span><span class="sxs-lookup"><span data-stu-id="c3ff3-139">String</span></span>|<span data-ttu-id="c3ff3-140">ペイロードファイル名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="c3ff3-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="c3ff3-141">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-141">\*.xml).</span></span>|
|<span data-ttu-id="c3ff3-142">payload</span><span class="sxs-lookup"><span data-stu-id="c3ff3-142">payload</span></span>|<span data-ttu-id="c3ff3-143">Binary</span><span class="sxs-lookup"><span data-stu-id="c3ff3-143">Binary</span></span>|<span data-ttu-id="c3ff3-144">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-144">Payload.</span></span> <span data-ttu-id="c3ff3-145">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="c3ff3-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c3ff3-146">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c3ff3-146">roleScopeTagIds</span></span>|<span data-ttu-id="c3ff3-147">String collection</span><span class="sxs-lookup"><span data-stu-id="c3ff3-147">String collection</span></span>|<span data-ttu-id="c3ff3-148">この iOS LOB アプリプロビジョニング構成エンティティのスコープタグのリスト。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-148">List of Scope Tags for this iOS LOB app provisioning configuration entity.</span></span>|
|<span data-ttu-id="c3ff3-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3ff3-149">createdDateTime</span></span>|<span data-ttu-id="c3ff3-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3ff3-150">DateTimeOffset</span></span>|<span data-ttu-id="c3ff3-151">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-151">DateTime the object was created.</span></span>|
|<span data-ttu-id="c3ff3-152">説明</span><span class="sxs-lookup"><span data-stu-id="c3ff3-152">description</span></span>|<span data-ttu-id="c3ff3-153">String</span><span class="sxs-lookup"><span data-stu-id="c3ff3-153">String</span></span>|<span data-ttu-id="c3ff3-154">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-154">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c3ff3-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3ff3-155">lastModifiedDateTime</span></span>|<span data-ttu-id="c3ff3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3ff3-156">DateTimeOffset</span></span>|<span data-ttu-id="c3ff3-157">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-157">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c3ff3-158">displayName</span><span class="sxs-lookup"><span data-stu-id="c3ff3-158">displayName</span></span>|<span data-ttu-id="c3ff3-159">String</span><span class="sxs-lookup"><span data-stu-id="c3ff3-159">String</span></span>|<span data-ttu-id="c3ff3-160">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-160">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c3ff3-161">version</span><span class="sxs-lookup"><span data-stu-id="c3ff3-161">version</span></span>|<span data-ttu-id="c3ff3-162">Int32</span><span class="sxs-lookup"><span data-stu-id="c3ff3-162">Int32</span></span>|<span data-ttu-id="c3ff3-163">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-163">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c3ff3-164">応答</span><span class="sxs-lookup"><span data-stu-id="c3ff3-164">Response</span></span>
<span data-ttu-id="c3ff3-165">成功した場合、このメソッド`200 OK`は応答コードと、更新された[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-165">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3ff3-166">例</span><span class="sxs-lookup"><span data-stu-id="c3ff3-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3ff3-167">要求</span><span class="sxs-lookup"><span data-stu-id="c3ff3-167">Request</span></span>
<span data-ttu-id="c3ff3-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-168">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3ff3-169">応答</span><span class="sxs-lookup"><span data-stu-id="c3ff3-169">Response</span></span>
<span data-ttu-id="c3ff3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3ff3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





