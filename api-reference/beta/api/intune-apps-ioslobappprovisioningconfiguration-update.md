---
title: ioslobappプロビジョニング構成の更新
description: ioslobappプロビジョニング構成オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 191df244cf163d0a5980c9fc0c5ae3a444e3468c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30173088"
---
# <a name="update-ioslobappprovisioningconfiguration"></a><span data-ttu-id="fa34a-103">ioslobappプロビジョニング構成の更新</span><span class="sxs-lookup"><span data-stu-id="fa34a-103">Update iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="fa34a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa34a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fa34a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fa34a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fa34a-106">[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="fa34a-106">Update the properties of a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fa34a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa34a-107">Prerequisites</span></span>
<span data-ttu-id="fa34a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa34a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fa34a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa34a-110">Permission type</span></span>|<span data-ttu-id="fa34a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa34a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa34a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa34a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fa34a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa34a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fa34a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa34a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa34a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa34a-115">Not supported.</span></span>|
|<span data-ttu-id="fa34a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa34a-116">Application</span></span>|<span data-ttu-id="fa34a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa34a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa34a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa34a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="fa34a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa34a-119">Request headers</span></span>
|<span data-ttu-id="fa34a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa34a-120">Header</span></span>|<span data-ttu-id="fa34a-121">値</span><span class="sxs-lookup"><span data-stu-id="fa34a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa34a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa34a-122">Authorization</span></span>|<span data-ttu-id="fa34a-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fa34a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa34a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fa34a-124">Accept</span></span>|<span data-ttu-id="fa34a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fa34a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa34a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa34a-126">Request body</span></span>
<span data-ttu-id="fa34a-127">要求本文で、 [ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fa34a-127">In the request body, supply a JSON representation for the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>

<span data-ttu-id="fa34a-128">次の表に、 [ioslobapp/構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fa34a-128">The following table shows the properties that are required when you create the [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md).</span></span>

|<span data-ttu-id="fa34a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa34a-129">Property</span></span>|<span data-ttu-id="fa34a-130">型</span><span class="sxs-lookup"><span data-stu-id="fa34a-130">Type</span></span>|<span data-ttu-id="fa34a-131">説明</span><span class="sxs-lookup"><span data-stu-id="fa34a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fa34a-132">id</span><span class="sxs-lookup"><span data-stu-id="fa34a-132">id</span></span>|<span data-ttu-id="fa34a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="fa34a-133">String</span></span>|<span data-ttu-id="fa34a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fa34a-134">Key of the entity.</span></span>|
|<span data-ttu-id="fa34a-135">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fa34a-135">expirationDateTime</span></span>|<span data-ttu-id="fa34a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa34a-136">DateTimeOffset</span></span>|<span data-ttu-id="fa34a-137">オプションのプロファイルの有効期限の日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="fa34a-137">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="fa34a-138">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="fa34a-138">payloadFileName</span></span>|<span data-ttu-id="fa34a-139">String</span><span class="sxs-lookup"><span data-stu-id="fa34a-139">String</span></span>|<span data-ttu-id="fa34a-140">ペイロードファイル名 (\*. mobileprovision</span><span class="sxs-lookup"><span data-stu-id="fa34a-140">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="fa34a-141">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="fa34a-141">\*.xml).</span></span>|
|<span data-ttu-id="fa34a-142">payload</span><span class="sxs-lookup"><span data-stu-id="fa34a-142">payload</span></span>|<span data-ttu-id="fa34a-143">Binary</span><span class="sxs-lookup"><span data-stu-id="fa34a-143">Binary</span></span>|<span data-ttu-id="fa34a-144">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="fa34a-144">Payload.</span></span> <span data-ttu-id="fa34a-145">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="fa34a-145">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="fa34a-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fa34a-146">createdDateTime</span></span>|<span data-ttu-id="fa34a-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa34a-147">DateTimeOffset</span></span>|<span data-ttu-id="fa34a-148">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fa34a-148">DateTime the object was created.</span></span>|
|<span data-ttu-id="fa34a-149">説明</span><span class="sxs-lookup"><span data-stu-id="fa34a-149">description</span></span>|<span data-ttu-id="fa34a-150">文字列</span><span class="sxs-lookup"><span data-stu-id="fa34a-150">String</span></span>|<span data-ttu-id="fa34a-151">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="fa34a-151">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="fa34a-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fa34a-152">lastModifiedDateTime</span></span>|<span data-ttu-id="fa34a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fa34a-153">DateTimeOffset</span></span>|<span data-ttu-id="fa34a-154">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fa34a-154">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="fa34a-155">displayName</span><span class="sxs-lookup"><span data-stu-id="fa34a-155">displayName</span></span>|<span data-ttu-id="fa34a-156">String</span><span class="sxs-lookup"><span data-stu-id="fa34a-156">String</span></span>|<span data-ttu-id="fa34a-157">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="fa34a-157">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="fa34a-158">version</span><span class="sxs-lookup"><span data-stu-id="fa34a-158">version</span></span>|<span data-ttu-id="fa34a-159">Int32</span><span class="sxs-lookup"><span data-stu-id="fa34a-159">Int32</span></span>|<span data-ttu-id="fa34a-160">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fa34a-160">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="fa34a-161">応答</span><span class="sxs-lookup"><span data-stu-id="fa34a-161">Response</span></span>
<span data-ttu-id="fa34a-162">成功した場合、このメソッド`200 OK`は応答コードと、更新された[ioslobappプロビジョニング構成](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="fa34a-162">If successful, this method returns a `200 OK` response code and an updated [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa34a-163">例</span><span class="sxs-lookup"><span data-stu-id="fa34a-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa34a-164">要求</span><span class="sxs-lookup"><span data-stu-id="fa34a-164">Request</span></span>
<span data-ttu-id="fa34a-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa34a-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
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

### <a name="response"></a><span data-ttu-id="fa34a-166">応答</span><span class="sxs-lookup"><span data-stu-id="fa34a-166">Response</span></span>
<span data-ttu-id="fa34a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa34a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




