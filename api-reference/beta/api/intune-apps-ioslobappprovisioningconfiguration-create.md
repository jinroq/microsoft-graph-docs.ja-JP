---
title: IosLobAppProvisioningConfiguration を作成します。
description: 新しい iosLobAppProvisioningConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d5a39a91156ebba649a3463568517d9b55a7fdfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944762"
---
# <a name="create-ioslobappprovisioningconfiguration"></a><span data-ttu-id="609fd-103">IosLobAppProvisioningConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="609fd-103">Create iosLobAppProvisioningConfiguration</span></span>

> <span data-ttu-id="609fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="609fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="609fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="609fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="609fd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="609fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="609fd-107">新しい[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="609fd-107">Create a new [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="609fd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="609fd-108">Prerequisites</span></span>
<span data-ttu-id="609fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="609fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="609fd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="609fd-111">Permission type</span></span>|<span data-ttu-id="609fd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="609fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="609fd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="609fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="609fd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="609fd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="609fd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="609fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="609fd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="609fd-116">Not supported.</span></span>|
|<span data-ttu-id="609fd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="609fd-117">Application</span></span>|<span data-ttu-id="609fd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="609fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="609fd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="609fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosLobAppProvisioningConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="609fd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="609fd-120">Request headers</span></span>
|<span data-ttu-id="609fd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="609fd-121">Header</span></span>|<span data-ttu-id="609fd-122">値</span><span class="sxs-lookup"><span data-stu-id="609fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="609fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="609fd-123">Authorization</span></span>|<span data-ttu-id="609fd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="609fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="609fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="609fd-125">Accept</span></span>|<span data-ttu-id="609fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="609fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="609fd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="609fd-127">Request body</span></span>
<span data-ttu-id="609fd-128">要求の本文に iosLobAppProvisioningConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="609fd-128">In the request body, supply a JSON representation for the iosLobAppProvisioningConfiguration object.</span></span>

<span data-ttu-id="609fd-129">次の表は、iosLobAppProvisioningConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="609fd-129">The following table shows the properties that are required when you create the iosLobAppProvisioningConfiguration.</span></span>

|<span data-ttu-id="609fd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="609fd-130">Property</span></span>|<span data-ttu-id="609fd-131">型</span><span class="sxs-lookup"><span data-stu-id="609fd-131">Type</span></span>|<span data-ttu-id="609fd-132">説明</span><span class="sxs-lookup"><span data-stu-id="609fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="609fd-133">ID</span><span class="sxs-lookup"><span data-stu-id="609fd-133">id</span></span>|<span data-ttu-id="609fd-134">String</span><span class="sxs-lookup"><span data-stu-id="609fd-134">String</span></span>|<span data-ttu-id="609fd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="609fd-135">Key of the entity.</span></span>|
|<span data-ttu-id="609fd-136">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="609fd-136">expirationDateTime</span></span>|<span data-ttu-id="609fd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="609fd-137">DateTimeOffset</span></span>|<span data-ttu-id="609fd-138">省略可能なプロファイルの有効期限の日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="609fd-138">Optional profile expiration date and time.</span></span>|
|<span data-ttu-id="609fd-139">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="609fd-139">payloadFileName</span></span>|<span data-ttu-id="609fd-140">String</span><span class="sxs-lookup"><span data-stu-id="609fd-140">String</span></span>|<span data-ttu-id="609fd-141">ペイロード ファイル名 (\*.mobileprovision</span><span class="sxs-lookup"><span data-stu-id="609fd-141">Payload file name (\*.mobileprovision</span></span> | <span data-ttu-id="609fd-142">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="609fd-142">\*.xml).</span></span>|
|<span data-ttu-id="609fd-143">payload</span><span class="sxs-lookup"><span data-stu-id="609fd-143">payload</span></span>|<span data-ttu-id="609fd-144">Binary</span><span class="sxs-lookup"><span data-stu-id="609fd-144">Binary</span></span>|<span data-ttu-id="609fd-145">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="609fd-145">Payload.</span></span> <span data-ttu-id="609fd-146">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="609fd-146">(UTF8 encoded byte array)</span></span>|
|<span data-ttu-id="609fd-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="609fd-147">createdDateTime</span></span>|<span data-ttu-id="609fd-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="609fd-148">DateTimeOffset</span></span>|<span data-ttu-id="609fd-149">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="609fd-149">DateTime the object was created.</span></span>|
|<span data-ttu-id="609fd-150">説明</span><span class="sxs-lookup"><span data-stu-id="609fd-150">description</span></span>|<span data-ttu-id="609fd-151">String</span><span class="sxs-lookup"><span data-stu-id="609fd-151">String</span></span>|<span data-ttu-id="609fd-152">デバイス構成について管理者が提供した説明です。</span><span class="sxs-lookup"><span data-stu-id="609fd-152">Admin provided description of the Device Configuration.</span></span>|
|<span data-ttu-id="609fd-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="609fd-153">lastModifiedDateTime</span></span>|<span data-ttu-id="609fd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="609fd-154">DateTimeOffset</span></span>|<span data-ttu-id="609fd-155">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="609fd-155">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="609fd-156">displayName</span><span class="sxs-lookup"><span data-stu-id="609fd-156">displayName</span></span>|<span data-ttu-id="609fd-157">String</span><span class="sxs-lookup"><span data-stu-id="609fd-157">String</span></span>|<span data-ttu-id="609fd-158">デバイス構成について管理者が指定した名前です。</span><span class="sxs-lookup"><span data-stu-id="609fd-158">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="609fd-159">version</span><span class="sxs-lookup"><span data-stu-id="609fd-159">version</span></span>|<span data-ttu-id="609fd-160">Int32</span><span class="sxs-lookup"><span data-stu-id="609fd-160">Int32</span></span>|<span data-ttu-id="609fd-161">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="609fd-161">Version of the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="609fd-162">応答</span><span class="sxs-lookup"><span data-stu-id="609fd-162">Response</span></span>
<span data-ttu-id="609fd-163">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="609fd-163">If successful, this method returns a `201 Created` response code and a [iosLobAppProvisioningConfiguration](../resources/intune-apps-ioslobappprovisioningconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="609fd-164">例</span><span class="sxs-lookup"><span data-stu-id="609fd-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="609fd-165">要求</span><span class="sxs-lookup"><span data-stu-id="609fd-165">Request</span></span>
<span data-ttu-id="609fd-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="609fd-166">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations
Content-type: application/json
Content-length: 377

{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfiguration",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA==",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="609fd-167">応答</span><span class="sxs-lookup"><span data-stu-id="609fd-167">Response</span></span>
<span data-ttu-id="609fd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="609fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





