---
title: macOSDeviceFeaturesConfigurations のリスト
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 171bb943d9288efc1d7c80593dbcbe7f009f65f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423168"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="76aac-103">macOSDeviceFeaturesConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="76aac-103">List macOSDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="76aac-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76aac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="76aac-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76aac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="76aac-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76aac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76aac-107">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="76aac-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76aac-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="76aac-108">Prerequisites</span></span>
<span data-ttu-id="76aac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76aac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="76aac-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76aac-111">Permission type</span></span>|<span data-ttu-id="76aac-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76aac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76aac-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76aac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76aac-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76aac-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="76aac-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76aac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76aac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76aac-116">Not supported.</span></span>|
|<span data-ttu-id="76aac-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76aac-117">Application</span></span>|<span data-ttu-id="76aac-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76aac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76aac-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76aac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76aac-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76aac-120">Request headers</span></span>
|<span data-ttu-id="76aac-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76aac-121">Header</span></span>|<span data-ttu-id="76aac-122">値</span><span class="sxs-lookup"><span data-stu-id="76aac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76aac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76aac-123">Authorization</span></span>|<span data-ttu-id="76aac-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="76aac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76aac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="76aac-125">Accept</span></span>|<span data-ttu-id="76aac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76aac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76aac-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="76aac-127">Request body</span></span>
<span data-ttu-id="76aac-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76aac-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76aac-129">応答</span><span class="sxs-lookup"><span data-stu-id="76aac-129">Response</span></span>
<span data-ttu-id="76aac-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="76aac-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76aac-131">例</span><span class="sxs-lookup"><span data-stu-id="76aac-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="76aac-132">要求</span><span class="sxs-lookup"><span data-stu-id="76aac-132">Request</span></span>
<span data-ttu-id="76aac-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76aac-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="76aac-134">応答</span><span class="sxs-lookup"><span data-stu-id="76aac-134">Response</span></span>
<span data-ttu-id="76aac-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76aac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




