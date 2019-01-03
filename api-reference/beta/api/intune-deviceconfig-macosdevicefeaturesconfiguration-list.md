---
title: macOSDeviceFeaturesConfigurations のリスト
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 8ac4c7ad035f973ebd0ad4a5c3d17a51a8f75f5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325516"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="620d1-103">macOSDeviceFeaturesConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="620d1-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="620d1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="620d1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="620d1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="620d1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="620d1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="620d1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="620d1-107">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="620d1-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="620d1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="620d1-108">Prerequisites</span></span>
<span data-ttu-id="620d1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="620d1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="620d1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="620d1-111">Permission type</span></span>|<span data-ttu-id="620d1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="620d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="620d1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="620d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="620d1-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="620d1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="620d1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="620d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="620d1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="620d1-116">Not supported.</span></span>|
|<span data-ttu-id="620d1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="620d1-117">Application</span></span>|<span data-ttu-id="620d1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="620d1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="620d1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="620d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="620d1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="620d1-120">Request headers</span></span>
|<span data-ttu-id="620d1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="620d1-121">Header</span></span>|<span data-ttu-id="620d1-122">値</span><span class="sxs-lookup"><span data-stu-id="620d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="620d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="620d1-123">Authorization</span></span>|<span data-ttu-id="620d1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="620d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="620d1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="620d1-125">Accept</span></span>|<span data-ttu-id="620d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="620d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="620d1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="620d1-127">Request body</span></span>
<span data-ttu-id="620d1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="620d1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="620d1-129">応答</span><span class="sxs-lookup"><span data-stu-id="620d1-129">Response</span></span>
<span data-ttu-id="620d1-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="620d1-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="620d1-131">例</span><span class="sxs-lookup"><span data-stu-id="620d1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="620d1-132">要求</span><span class="sxs-lookup"><span data-stu-id="620d1-132">Request</span></span>
<span data-ttu-id="620d1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="620d1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="620d1-134">応答</span><span class="sxs-lookup"><span data-stu-id="620d1-134">Response</span></span>
<span data-ttu-id="620d1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="620d1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 785

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
      "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ]
    }
  ]
}
```




