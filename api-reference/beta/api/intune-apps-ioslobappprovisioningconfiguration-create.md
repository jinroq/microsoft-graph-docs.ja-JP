---
title: ioslobappプロビジョニング構成を作成する
description: 新しい ioslobappプロビジョニング構成オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 08a3cb70d7fc10274e44550d83da252710d9ec9d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171527"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="c3a53-103">ioslobappプロビジョニング構成を作成する</span><span class="sxs-lookup"><span data-stu-id="c3a53-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="c3a53-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3a53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a53-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3a53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a53-106">新しい[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3a53-106">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3a53-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3a53-107">Prerequisites</span></span>
<span data-ttu-id="c3a53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3a53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c3a53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3a53-110">Permission type</span></span>|<span data-ttu-id="c3a53-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3a53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3a53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3a53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3a53-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a53-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3a53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3a53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3a53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3a53-115">Not supported.</span></span>|
|<span data-ttu-id="c3a53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3a53-116">Application</span></span>|<span data-ttu-id="c3a53-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3a53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3a53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3a53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c3a53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3a53-119">Request headers</span></span>
|<span data-ttu-id="c3a53-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3a53-120">Header</span></span>|<span data-ttu-id="c3a53-121">値</span><span class="sxs-lookup"><span data-stu-id="c3a53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3a53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3a53-122">Authorization</span></span>|<span data-ttu-id="c3a53-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c3a53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3a53-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c3a53-124">Accept</span></span>|<span data-ttu-id="c3a53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3a53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3a53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3a53-126">Request body</span></span>
<span data-ttu-id="c3a53-127">要求本文で、ioslobappプロビジョニング構成オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3a53-127">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="c3a53-128">次の表に、ioslobapp/構成の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3a53-128">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="c3a53-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3a53-129">Property</span></span>|<span data-ttu-id="c3a53-130">型</span><span class="sxs-lookup"><span data-stu-id="c3a53-130">Type</span></span>|<span data-ttu-id="c3a53-131">説明</span><span class="sxs-lookup"><span data-stu-id="c3a53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a53-132">id</span><span class="sxs-lookup"><span data-stu-id="c3a53-132">id</span></span>|<span data-ttu-id="c3a53-133">文字列</span><span class="sxs-lookup"><span data-stu-id="c3a53-133">String</span></span>|<span data-ttu-id="c3a53-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3a53-134">Key of the entity.</span></span>|
|<span data-ttu-id="c3a53-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c3a53-135">expirationDateTime</span></span>|<span data-ttu-id="c3a53-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a53-136">DateTimeOffset</span></span>|<span data-ttu-id="c3a53-137">オプションのプロファイルの有効期限の日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c3a53-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="c3a53-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="c3a53-138">payloadFileName</span></span>|<span data-ttu-id="c3a53-139">String</span><span class="sxs-lookup"><span data-stu-id="c3a53-139">String</span></span>|<span data-ttu-id="c3a53-140">ペイロードファイル名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="c3a53-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="c3a53-141">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="c3a53-141">\*.xml).</span></span>|
|<span data-ttu-id="c3a53-142">payload</span><span class="sxs-lookup"><span data-stu-id="c3a53-142">payload</span></span>|<span data-ttu-id="c3a53-143">Binary</span><span class="sxs-lookup"><span data-stu-id="c3a53-143">Binary</span></span>|<span data-ttu-id="c3a53-144">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="c3a53-144">Payload.</span></span> <span data-ttu-id="c3a53-145">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="c3a53-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="c3a53-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3a53-146">createdDateTime</span></span>|<span data-ttu-id="c3a53-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a53-147">DateTimeOffset</span></span>|<span data-ttu-id="c3a53-148">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3a53-148">DateTime the object was created.</span></span>|
|<span data-ttu-id="c3a53-149">説明</span><span class="sxs-lookup"><span data-stu-id="c3a53-149">description</span></span>|<span data-ttu-id="c3a53-150">文字列</span><span class="sxs-lookup"><span data-stu-id="c3a53-150">String</span></span>|<span data-ttu-id="c3a53-151">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="c3a53-151">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="c3a53-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c3a53-152">lastModifiedDateTime</span></span>|<span data-ttu-id="c3a53-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3a53-153">DateTimeOffset</span></span>|<span data-ttu-id="c3a53-154">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c3a53-154">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c3a53-155">displayName</span><span class="sxs-lookup"><span data-stu-id="c3a53-155">displayName</span></span>|<span data-ttu-id="c3a53-156">String</span><span class="sxs-lookup"><span data-stu-id="c3a53-156">String</span></span>|<span data-ttu-id="c3a53-157">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="c3a53-157">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c3a53-158">version</span><span class="sxs-lookup"><span data-stu-id="c3a53-158">version</span></span>|<span data-ttu-id="c3a53-159">Int32</span><span class="sxs-lookup"><span data-stu-id="c3a53-159">Int32</span></span>|<span data-ttu-id="c3a53-160">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c3a53-160">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c3a53-161">応答</span><span class="sxs-lookup"><span data-stu-id="c3a53-161">Response</span></span>
<span data-ttu-id="c3a53-162">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3a53-162">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3a53-163">例</span><span class="sxs-lookup"><span data-stu-id="c3a53-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3a53-164">要求</span><span class="sxs-lookup"><span data-stu-id="c3a53-164">Request</span></span>
<span data-ttu-id="c3a53-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3a53-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="c3a53-166">応答</span><span class="sxs-lookup"><span data-stu-id="c3a53-166">Response</span></span>
<span data-ttu-id="c3a53-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3a53-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 485

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "id": "e2a23631-3631-e2a2-3136-a2e23136a2e2",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```




