---
title: DataSharingConsent を作成します。
description: 新しい dataSharingConsent オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 07d76bbd92d2741571683bb7614b3336c10d9058
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349673"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="8cb3d-103">DataSharingConsent を作成します。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="8cb3d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cb3d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cb3d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8cb3d-107">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-107">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8cb3d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8cb3d-108">Prerequisites</span></span>
<span data-ttu-id="8cb3d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cb3d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cb3d-111">Permission type</span></span>|<span data-ttu-id="8cb3d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cb3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cb3d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cb3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8cb3d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cb3d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8cb3d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cb3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cb3d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-116">Not supported.</span></span>|
|<span data-ttu-id="8cb3d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cb3d-117">Application</span></span>|<span data-ttu-id="8cb3d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cb3d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cb3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="8cb3d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cb3d-120">Request headers</span></span>
|<span data-ttu-id="8cb3d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cb3d-121">Header</span></span>|<span data-ttu-id="8cb3d-122">値</span><span class="sxs-lookup"><span data-stu-id="8cb3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cb3d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cb3d-123">Authorization</span></span>|<span data-ttu-id="8cb3d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cb3d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8cb3d-125">Accept</span></span>|<span data-ttu-id="8cb3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8cb3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cb3d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cb3d-127">Request body</span></span>
<span data-ttu-id="8cb3d-128">要求の本文に dataSharingConsent オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-128">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="8cb3d-129">次の表は、dataSharingConsent を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-129">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="8cb3d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cb3d-130">Property</span></span>|<span data-ttu-id="8cb3d-131">種類</span><span class="sxs-lookup"><span data-stu-id="8cb3d-131">Type</span></span>|<span data-ttu-id="8cb3d-132">説明</span><span class="sxs-lookup"><span data-stu-id="8cb3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cb3d-133">ID</span><span class="sxs-lookup"><span data-stu-id="8cb3d-133">id</span></span>|<span data-ttu-id="8cb3d-134">String</span><span class="sxs-lookup"><span data-stu-id="8cb3d-134">String</span></span>|<span data-ttu-id="8cb3d-135">データ共有同意 Id</span><span class="sxs-lookup"><span data-stu-id="8cb3d-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="8cb3d-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8cb3d-136">serviceDisplayName</span></span>|<span data-ttu-id="8cb3d-137">String</span><span class="sxs-lookup"><span data-stu-id="8cb3d-137">String</span></span>|<span data-ttu-id="8cb3d-138">サービス作業の流れの表示名</span><span class="sxs-lookup"><span data-stu-id="8cb3d-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="8cb3d-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="8cb3d-139">termsUrl</span></span>|<span data-ttu-id="8cb3d-140">String</span><span class="sxs-lookup"><span data-stu-id="8cb3d-140">String</span></span>|<span data-ttu-id="8cb3d-141">同意の共有データの TermsUrl</span><span class="sxs-lookup"><span data-stu-id="8cb3d-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="8cb3d-142">付与</span><span class="sxs-lookup"><span data-stu-id="8cb3d-142">granted</span></span>|<span data-ttu-id="8cb3d-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="8cb3d-143">Boolean</span></span>|<span data-ttu-id="8cb3d-144">同意の共有データに付与されている状態</span><span class="sxs-lookup"><span data-stu-id="8cb3d-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="8cb3d-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="8cb3d-145">grantDateTime</span></span>|<span data-ttu-id="8cb3d-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cb3d-146">DateTimeOffset</span></span>|<span data-ttu-id="8cb3d-147">同意は、このアカウントに与えられました。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="8cb3d-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="8cb3d-148">grantedByUpn</span></span>|<span data-ttu-id="8cb3d-149">String</span><span class="sxs-lookup"><span data-stu-id="8cb3d-149">String</span></span>|<span data-ttu-id="8cb3d-150">このアカウントに許可を付与するユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="8cb3d-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="8cb3d-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="8cb3d-151">grantedByUserId</span></span>|<span data-ttu-id="8cb3d-152">String</span><span class="sxs-lookup"><span data-stu-id="8cb3d-152">String</span></span>|<span data-ttu-id="8cb3d-153">このアカウントに許可を付与するユーザーのユーザー Id</span><span class="sxs-lookup"><span data-stu-id="8cb3d-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="8cb3d-154">応答</span><span class="sxs-lookup"><span data-stu-id="8cb3d-154">Response</span></span>
<span data-ttu-id="8cb3d-155">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-155">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cb3d-156">例</span><span class="sxs-lookup"><span data-stu-id="8cb3d-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="8cb3d-157">要求</span><span class="sxs-lookup"><span data-stu-id="8cb3d-157">Request</span></span>
<span data-ttu-id="8cb3d-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```

### <a name="response"></a><span data-ttu-id="8cb3d-159">応答</span><span class="sxs-lookup"><span data-stu-id="8cb3d-159">Response</span></span>
<span data-ttu-id="8cb3d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cb3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "333387f7-87f7-3333-f787-3333f7873333",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```




