---
title: macOSGeneralDeviceConfigurations のリスト
description: macOSGeneralDeviceConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5fba74eaa8f8c59f46d636d9095a7675f3c6190
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997401"
---
# <a name="list-macosgeneraldeviceconfigurations"></a><span data-ttu-id="4c552-103">macOSGeneralDeviceConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="4c552-103">List macOSGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="4c552-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c552-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c552-105">[macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4c552-105">List properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c552-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c552-106">Prerequisites</span></span>
<span data-ttu-id="4c552-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c552-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c552-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c552-109">Permission type</span></span>|<span data-ttu-id="4c552-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c552-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c552-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c552-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4c552-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4c552-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4c552-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c552-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c552-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c552-114">Not supported.</span></span>|
|<span data-ttu-id="4c552-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c552-115">Application</span></span>|<span data-ttu-id="4c552-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c552-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c552-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c552-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c552-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c552-118">Request headers</span></span>
|<span data-ttu-id="4c552-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c552-119">Header</span></span>|<span data-ttu-id="4c552-120">値</span><span class="sxs-lookup"><span data-stu-id="4c552-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c552-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c552-121">Authorization</span></span>|<span data-ttu-id="4c552-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c552-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c552-123">承諾</span><span class="sxs-lookup"><span data-stu-id="4c552-123">Accept</span></span>|<span data-ttu-id="4c552-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4c552-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c552-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c552-125">Request body</span></span>
<span data-ttu-id="4c552-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4c552-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c552-127">応答</span><span class="sxs-lookup"><span data-stu-id="4c552-127">Response</span></span>
<span data-ttu-id="4c552-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4c552-128">If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c552-129">例</span><span class="sxs-lookup"><span data-stu-id="4c552-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c552-130">要求</span><span class="sxs-lookup"><span data-stu-id="4c552-130">Request</span></span>
<span data-ttu-id="4c552-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c552-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="4c552-132">応答</span><span class="sxs-lookup"><span data-stu-id="4c552-132">Response</span></span>
<span data-ttu-id="4c552-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c552-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1227

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "emailInDomainSuffixes": [
        "Email In Domain Suffixes value"
      ],
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumCharacterSetCount": 0,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true
    }
  ]
}
```



