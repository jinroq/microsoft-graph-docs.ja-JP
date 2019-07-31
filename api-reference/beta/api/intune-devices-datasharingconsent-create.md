---
title: DataSharingConsent を作成する
description: 新しい dataSharingConsent オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b569e19baf9265be6d4937f6d6c025cb80730cb8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986184"
---
# <a name="create-datasharingconsent"></a><span data-ttu-id="cfeec-103">DataSharingConsent を作成する</span><span class="sxs-lookup"><span data-stu-id="cfeec-103">Create dataSharingConsent</span></span>

> <span data-ttu-id="cfeec-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfeec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfeec-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfeec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfeec-106">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cfeec-106">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cfeec-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="cfeec-107">Prerequisites</span></span>
<span data-ttu-id="cfeec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cfeec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfeec-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cfeec-110">Permission type</span></span>|<span data-ttu-id="cfeec-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cfeec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cfeec-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cfeec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cfeec-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfeec-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="cfeec-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cfeec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cfeec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfeec-115">Not supported.</span></span>|
|<span data-ttu-id="cfeec-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cfeec-116">Application</span></span>|<span data-ttu-id="cfeec-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cfeec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cfeec-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cfeec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents
```

## <a name="request-headers"></a><span data-ttu-id="cfeec-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfeec-119">Request headers</span></span>
|<span data-ttu-id="cfeec-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cfeec-120">Header</span></span>|<span data-ttu-id="cfeec-121">値</span><span class="sxs-lookup"><span data-stu-id="cfeec-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cfeec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cfeec-122">Authorization</span></span>|<span data-ttu-id="cfeec-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="cfeec-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cfeec-124">承諾</span><span class="sxs-lookup"><span data-stu-id="cfeec-124">Accept</span></span>|<span data-ttu-id="cfeec-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cfeec-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cfeec-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="cfeec-126">Request body</span></span>
<span data-ttu-id="cfeec-127">要求本文で、dataSharingConsent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cfeec-127">In the request body, supply a JSON representation for the dataSharingConsent object.</span></span>

<span data-ttu-id="cfeec-128">次の表に、dataSharingConsent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cfeec-128">The following table shows the properties that are required when you create the dataSharingConsent.</span></span>

|<span data-ttu-id="cfeec-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cfeec-129">Property</span></span>|<span data-ttu-id="cfeec-130">型</span><span class="sxs-lookup"><span data-stu-id="cfeec-130">Type</span></span>|<span data-ttu-id="cfeec-131">説明</span><span class="sxs-lookup"><span data-stu-id="cfeec-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfeec-132">id</span><span class="sxs-lookup"><span data-stu-id="cfeec-132">id</span></span>|<span data-ttu-id="cfeec-133">String</span><span class="sxs-lookup"><span data-stu-id="cfeec-133">String</span></span>|<span data-ttu-id="cfeec-134">データ共有の同意 Id</span><span class="sxs-lookup"><span data-stu-id="cfeec-134">The data sharing consent Id</span></span>|
|<span data-ttu-id="cfeec-135">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="cfeec-135">serviceDisplayName</span></span>|<span data-ttu-id="cfeec-136">String</span><span class="sxs-lookup"><span data-stu-id="cfeec-136">String</span></span>|<span data-ttu-id="cfeec-137">サービスワークフローの表示名</span><span class="sxs-lookup"><span data-stu-id="cfeec-137">The display name of the service work flow</span></span>|
|<span data-ttu-id="cfeec-138">termsUrl</span><span class="sxs-lookup"><span data-stu-id="cfeec-138">termsUrl</span></span>|<span data-ttu-id="cfeec-139">String</span><span class="sxs-lookup"><span data-stu-id="cfeec-139">String</span></span>|<span data-ttu-id="cfeec-140">データ共有の同意の TermsUrl</span><span class="sxs-lookup"><span data-stu-id="cfeec-140">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="cfeec-141">granted</span><span class="sxs-lookup"><span data-stu-id="cfeec-141">granted</span></span>|<span data-ttu-id="cfeec-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="cfeec-142">Boolean</span></span>|<span data-ttu-id="cfeec-143">データ共有の同意の付与された状態</span><span class="sxs-lookup"><span data-stu-id="cfeec-143">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="cfeec-144">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="cfeec-144">grantDateTime</span></span>|<span data-ttu-id="cfeec-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cfeec-145">DateTimeOffset</span></span>|<span data-ttu-id="cfeec-146">このアカウントに対して同意が与えられた時間</span><span class="sxs-lookup"><span data-stu-id="cfeec-146">The time consent was granted for this account</span></span>|
|<span data-ttu-id="cfeec-147">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="cfeec-147">grantedByUpn</span></span>|<span data-ttu-id="cfeec-148">String</span><span class="sxs-lookup"><span data-stu-id="cfeec-148">String</span></span>|<span data-ttu-id="cfeec-149">このアカウントに同意を付与したユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="cfeec-149">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="cfeec-150">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="cfeec-150">grantedByUserId</span></span>|<span data-ttu-id="cfeec-151">String</span><span class="sxs-lookup"><span data-stu-id="cfeec-151">String</span></span>|<span data-ttu-id="cfeec-152">このアカウントに同意を付与したユーザーの UserId</span><span class="sxs-lookup"><span data-stu-id="cfeec-152">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="cfeec-153">応答</span><span class="sxs-lookup"><span data-stu-id="cfeec-153">Response</span></span>
<span data-ttu-id="cfeec-154">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cfeec-154">If successful, this method returns a `201 Created` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfeec-155">例</span><span class="sxs-lookup"><span data-stu-id="cfeec-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="cfeec-156">要求</span><span class="sxs-lookup"><span data-stu-id="cfeec-156">Request</span></span>
<span data-ttu-id="cfeec-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cfeec-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cfeec-158">応答</span><span class="sxs-lookup"><span data-stu-id="cfeec-158">Response</span></span>
<span data-ttu-id="cfeec-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cfeec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





