---
title: AndroidManagedStoreAccountEnterpriseSettings の取得
description: AndroidManagedStoreAccountEnterpriseSettings オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad7e0b7f374404fdb651ba778e2e2382d3ae4a04
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322752"
---
# <a name="get-androidmanagedstoreaccountenterprisesettings"></a><span data-ttu-id="e2570-103">AndroidManagedStoreAccountEnterpriseSettings の取得</span><span class="sxs-lookup"><span data-stu-id="e2570-103">Get androidManagedStoreAccountEnterpriseSettings</span></span>

> <span data-ttu-id="e2570-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2570-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2570-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2570-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2570-106">[Androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e2570-106">Read properties and relationships of the [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2570-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e2570-107">Prerequisites</span></span>
<span data-ttu-id="e2570-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2570-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2570-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2570-110">Permission type</span></span>|<span data-ttu-id="e2570-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2570-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2570-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2570-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e2570-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2570-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e2570-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2570-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2570-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2570-115">Not supported.</span></span>|
|<span data-ttu-id="e2570-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2570-116">Application</span></span>|<span data-ttu-id="e2570-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2570-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2570-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2570-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e2570-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e2570-119">Optional query parameters</span></span>
<span data-ttu-id="e2570-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e2570-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2570-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2570-121">Request headers</span></span>
|<span data-ttu-id="e2570-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2570-122">Header</span></span>|<span data-ttu-id="e2570-123">値</span><span class="sxs-lookup"><span data-stu-id="e2570-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2570-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2570-124">Authorization</span></span>|<span data-ttu-id="e2570-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e2570-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2570-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e2570-126">Accept</span></span>|<span data-ttu-id="e2570-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e2570-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2570-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2570-128">Request body</span></span>
<span data-ttu-id="e2570-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e2570-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2570-130">応答</span><span class="sxs-lookup"><span data-stu-id="e2570-130">Response</span></span>
<span data-ttu-id="e2570-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Androidmanagedstoreaccountenterprisesettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e2570-131">If successful, this method returns a `200 OK` response code and [androidManagedStoreAccountEnterpriseSettings](../resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2570-132">例</span><span class="sxs-lookup"><span data-stu-id="e2570-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2570-133">要求</span><span class="sxs-lookup"><span data-stu-id="e2570-133">Request</span></span>
<span data-ttu-id="e2570-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2570-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings
```

### <a name="response"></a><span data-ttu-id="e2570-135">応答</span><span class="sxs-lookup"><span data-stu-id="e2570-135">Response</span></span>
<span data-ttu-id="e2570-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2570-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1081

{
  "value": {
    "@odata.type": "#microsoft.graph.androidManagedStoreAccountEnterpriseSettings",
    "id": "b71357c9-57c9-b713-c957-13b7c95713b7",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true,
    "companyCodes": [
      {
        "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode",
        "enrollmentToken": "Enrollment Token value",
        "qrCodeContent": "Qr Code Content value",
        "qrCodeImage": {
          "@odata.type": "microsoft.graph.mimeContent",
          "type": "Type value",
          "value": "dmFsdWU="
        }
      }
    ],
    "androidDeviceOwnerFullyManagedEnrollmentEnabled": true
  }
}
```






