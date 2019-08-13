---
title: DataSharingConsent の更新
description: DataSharingConsent オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 073ab096a3bacdec1e01e44e891baa2802f5bd61
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310634"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="7f7c1-103">DataSharingConsent の更新</span><span class="sxs-lookup"><span data-stu-id="7f7c1-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="7f7c1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f7c1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f7c1-106">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-106">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f7c1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f7c1-107">Prerequisites</span></span>
<span data-ttu-id="7f7c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f7c1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f7c1-110">Permission type</span></span>|<span data-ttu-id="7f7c1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f7c1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f7c1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f7c1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f7c1-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7c1-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f7c1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f7c1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f7c1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-115">Not supported.</span></span>|
|<span data-ttu-id="7f7c1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f7c1-116">Application</span></span>|<span data-ttu-id="7f7c1-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f7c1-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f7c1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f7c1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="7f7c1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f7c1-119">Request headers</span></span>
|<span data-ttu-id="7f7c1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f7c1-120">Header</span></span>|<span data-ttu-id="7f7c1-121">値</span><span class="sxs-lookup"><span data-stu-id="7f7c1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f7c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f7c1-122">Authorization</span></span>|<span data-ttu-id="7f7c1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f7c1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7f7c1-124">Accept</span></span>|<span data-ttu-id="7f7c1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7f7c1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f7c1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f7c1-126">Request body</span></span>
<span data-ttu-id="7f7c1-127">要求本文で、 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-127">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="7f7c1-128">次の表に、 [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-128">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="7f7c1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f7c1-129">Property</span></span>|<span data-ttu-id="7f7c1-130">型</span><span class="sxs-lookup"><span data-stu-id="7f7c1-130">Type</span></span>|<span data-ttu-id="7f7c1-131">説明</span><span class="sxs-lookup"><span data-stu-id="7f7c1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f7c1-132">id</span><span class="sxs-lookup"><span data-stu-id="7f7c1-132">id</span></span>|<span data-ttu-id="7f7c1-133">String</span><span class="sxs-lookup"><span data-stu-id="7f7c1-133">String</span></span>|<span data-ttu-id="7f7c1-134">データ共有の同意 Id</span><span class="sxs-lookup"><span data-stu-id="7f7c1-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="7f7c1-135">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="7f7c1-135">serviceDisplayName</span></span>|<span data-ttu-id="7f7c1-136">String</span><span class="sxs-lookup"><span data-stu-id="7f7c1-136">String</span></span>|<span data-ttu-id="7f7c1-137">サービスワークフローの表示名</span><span class="sxs-lookup"><span data-stu-id="7f7c1-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="7f7c1-138">termsUrl</span><span class="sxs-lookup"><span data-stu-id="7f7c1-138">termsUrl</span></span>|<span data-ttu-id="7f7c1-139">String</span><span class="sxs-lookup"><span data-stu-id="7f7c1-139">String</span></span>|<span data-ttu-id="7f7c1-140">データ共有の同意の TermsUrl</span><span class="sxs-lookup"><span data-stu-id="7f7c1-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="7f7c1-141">granted</span><span class="sxs-lookup"><span data-stu-id="7f7c1-141">granted</span></span>|<span data-ttu-id="7f7c1-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f7c1-142">Boolean</span></span>|<span data-ttu-id="7f7c1-143">データ共有の同意の付与された状態</span><span class="sxs-lookup"><span data-stu-id="7f7c1-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="7f7c1-144">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="7f7c1-144">grantDateTime</span></span>|<span data-ttu-id="7f7c1-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f7c1-145">DateTimeOffset</span></span>|<span data-ttu-id="7f7c1-146">このアカウントに対して同意が与えられた時間</span><span class="sxs-lookup"><span data-stu-id="7f7c1-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="7f7c1-147">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="7f7c1-147">grantedByUpn</span></span>|<span data-ttu-id="7f7c1-148">String</span><span class="sxs-lookup"><span data-stu-id="7f7c1-148">String</span></span>|<span data-ttu-id="7f7c1-149">このアカウントに同意を付与したユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="7f7c1-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="7f7c1-150">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="7f7c1-150">grantedByUserId</span></span>|<span data-ttu-id="7f7c1-151">String</span><span class="sxs-lookup"><span data-stu-id="7f7c1-151">String</span></span>|<span data-ttu-id="7f7c1-152">このアカウントに同意を付与したユーザーの UserId</span><span class="sxs-lookup"><span data-stu-id="7f7c1-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="7f7c1-153">応答</span><span class="sxs-lookup"><span data-stu-id="7f7c1-153">Response</span></span>
<span data-ttu-id="7f7c1-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-154">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f7c1-155">例</span><span class="sxs-lookup"><span data-stu-id="7f7c1-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f7c1-156">要求</span><span class="sxs-lookup"><span data-stu-id="7f7c1-156">Request</span></span>
<span data-ttu-id="7f7c1-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
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

### <a name="response"></a><span data-ttu-id="7f7c1-158">応答</span><span class="sxs-lookup"><span data-stu-id="7f7c1-158">Response</span></span>
<span data-ttu-id="7f7c1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f7c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






