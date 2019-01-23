---
title: DataSharingConsent を更新します。
description: DataSharingConsent オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 143e2c655adac2403f49bb92afff2aca30a3653f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421117"
---
# <a name="update-datasharingconsent"></a><span data-ttu-id="e022b-103">DataSharingConsent を更新します。</span><span class="sxs-lookup"><span data-stu-id="e022b-103">Update dataSharingConsent</span></span>

> <span data-ttu-id="e022b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e022b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e022b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e022b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e022b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e022b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e022b-107">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e022b-107">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e022b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e022b-108">Prerequisites</span></span>
<span data-ttu-id="e022b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e022b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e022b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e022b-111">Permission type</span></span>|<span data-ttu-id="e022b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e022b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e022b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e022b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e022b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e022b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e022b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e022b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e022b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e022b-116">Not supported.</span></span>|
|<span data-ttu-id="e022b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e022b-117">Application</span></span>|<span data-ttu-id="e022b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e022b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e022b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e022b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## <a name="request-headers"></a><span data-ttu-id="e022b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e022b-120">Request headers</span></span>
|<span data-ttu-id="e022b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e022b-121">Header</span></span>|<span data-ttu-id="e022b-122">値</span><span class="sxs-lookup"><span data-stu-id="e022b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e022b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e022b-123">Authorization</span></span>|<span data-ttu-id="e022b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e022b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e022b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e022b-125">Accept</span></span>|<span data-ttu-id="e022b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e022b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e022b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e022b-127">Request body</span></span>
<span data-ttu-id="e022b-128">要求の本文に[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e022b-128">In the request body, supply a JSON representation for the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>

<span data-ttu-id="e022b-129">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="e022b-129">The following table shows the properties that are required when you create the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>

|<span data-ttu-id="e022b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e022b-130">Property</span></span>|<span data-ttu-id="e022b-131">型</span><span class="sxs-lookup"><span data-stu-id="e022b-131">Type</span></span>|<span data-ttu-id="e022b-132">説明</span><span class="sxs-lookup"><span data-stu-id="e022b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e022b-133">id</span><span class="sxs-lookup"><span data-stu-id="e022b-133">id</span></span>|<span data-ttu-id="e022b-134">String</span><span class="sxs-lookup"><span data-stu-id="e022b-134">String</span></span>|<span data-ttu-id="e022b-135">データ共有同意 Id</span><span class="sxs-lookup"><span data-stu-id="e022b-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="e022b-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e022b-136">serviceDisplayName</span></span>|<span data-ttu-id="e022b-137">String</span><span class="sxs-lookup"><span data-stu-id="e022b-137">String</span></span>|<span data-ttu-id="e022b-138">サービス作業の流れの表示名</span><span class="sxs-lookup"><span data-stu-id="e022b-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="e022b-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="e022b-139">termsUrl</span></span>|<span data-ttu-id="e022b-140">String</span><span class="sxs-lookup"><span data-stu-id="e022b-140">String</span></span>|<span data-ttu-id="e022b-141">同意の共有データの TermsUrl</span><span class="sxs-lookup"><span data-stu-id="e022b-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="e022b-142">付与</span><span class="sxs-lookup"><span data-stu-id="e022b-142">granted</span></span>|<span data-ttu-id="e022b-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e022b-143">Boolean</span></span>|<span data-ttu-id="e022b-144">同意の共有データに付与されている状態</span><span class="sxs-lookup"><span data-stu-id="e022b-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="e022b-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="e022b-145">grantDateTime</span></span>|<span data-ttu-id="e022b-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e022b-146">DateTimeOffset</span></span>|<span data-ttu-id="e022b-147">同意は、このアカウントに与えられました。</span><span class="sxs-lookup"><span data-stu-id="e022b-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="e022b-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="e022b-148">grantedByUpn</span></span>|<span data-ttu-id="e022b-149">String</span><span class="sxs-lookup"><span data-stu-id="e022b-149">String</span></span>|<span data-ttu-id="e022b-150">このアカウントに許可を付与するユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="e022b-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="e022b-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="e022b-151">grantedByUserId</span></span>|<span data-ttu-id="e022b-152">String</span><span class="sxs-lookup"><span data-stu-id="e022b-152">String</span></span>|<span data-ttu-id="e022b-153">このアカウントに許可を付与するユーザーのユーザー Id</span><span class="sxs-lookup"><span data-stu-id="e022b-153">The UserId of the user that granted consent for this account</span></span>|



## <a name="response"></a><span data-ttu-id="e022b-154">応答</span><span class="sxs-lookup"><span data-stu-id="e022b-154">Response</span></span>
<span data-ttu-id="e022b-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e022b-155">If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e022b-156">例</span><span class="sxs-lookup"><span data-stu-id="e022b-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="e022b-157">要求</span><span class="sxs-lookup"><span data-stu-id="e022b-157">Request</span></span>
<span data-ttu-id="e022b-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e022b-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e022b-159">応答</span><span class="sxs-lookup"><span data-stu-id="e022b-159">Response</span></span>
<span data-ttu-id="e022b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e022b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




