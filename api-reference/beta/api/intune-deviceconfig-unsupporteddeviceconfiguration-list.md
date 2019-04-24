---
title: 非 supporteddeviceconfigurウニを一覧表示する
description: 非 supporteddevic/オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be68994f7d333ed428039093fda1fb6b98e52af5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32517821"
---
# <a name="list-unsupporteddeviceconfigurations"></a><span data-ttu-id="689db-103">非 supporteddeviceconfigurウニを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="689db-103">List unsupportedDeviceConfigurations</span></span>

> <span data-ttu-id="689db-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="689db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689db-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="689db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689db-106">非[supporteddevic/](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="689db-106">List properties and relationships of the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="689db-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="689db-107">Prerequisites</span></span>
<span data-ttu-id="689db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="689db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="689db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="689db-110">Permission type</span></span>|<span data-ttu-id="689db-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="689db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="689db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="689db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="689db-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="689db-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="689db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="689db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="689db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="689db-115">Not supported.</span></span>|
|<span data-ttu-id="689db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="689db-116">Application</span></span>|<span data-ttu-id="689db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="689db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="689db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="689db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="689db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="689db-119">Request headers</span></span>
|<span data-ttu-id="689db-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="689db-120">Header</span></span>|<span data-ttu-id="689db-121">値</span><span class="sxs-lookup"><span data-stu-id="689db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="689db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="689db-122">Authorization</span></span>|<span data-ttu-id="689db-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="689db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="689db-124">承諾</span><span class="sxs-lookup"><span data-stu-id="689db-124">Accept</span></span>|<span data-ttu-id="689db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="689db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="689db-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="689db-126">Request body</span></span>
<span data-ttu-id="689db-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="689db-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="689db-128">応答</span><span class="sxs-lookup"><span data-stu-id="689db-128">Response</span></span>
<span data-ttu-id="689db-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アン supporteddevic/](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="689db-129">If successful, this method returns a `200 OK` response code and a collection of [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="689db-130">例</span><span class="sxs-lookup"><span data-stu-id="689db-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="689db-131">要求</span><span class="sxs-lookup"><span data-stu-id="689db-131">Request</span></span>
<span data-ttu-id="689db-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="689db-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="689db-133">応答</span><span class="sxs-lookup"><span data-stu-id="689db-133">Response</span></span>
<span data-ttu-id="689db-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="689db-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 799

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
      "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "originalEntityTypeName": "Original Entity Type Name value",
      "details": [
        {
          "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
          "message": "Message value",
          "propertyName": "Property Name value"
        }
      ]
    }
  ]
}
```





