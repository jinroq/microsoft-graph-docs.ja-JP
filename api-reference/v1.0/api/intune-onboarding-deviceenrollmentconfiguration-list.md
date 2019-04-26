---
title: deviceEnrollmentConfigurations のリスト
description: deviceEnrollmentConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ee88dd5674885944f89527bc028d6bb598fe298f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567376"
---
# <a name="list-deviceenrollmentconfigurations"></a><span data-ttu-id="eb593-103">deviceEnrollmentConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="eb593-103">List deviceEnrollmentConfigurations</span></span>

> <span data-ttu-id="eb593-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb593-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb593-105">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="eb593-105">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb593-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="eb593-106">Prerequisites</span></span>
<span data-ttu-id="eb593-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb593-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb593-109">Permission type</span></span>|<span data-ttu-id="eb593-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb593-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb593-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb593-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eb593-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb593-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="eb593-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb593-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb593-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb593-114">Not supported.</span></span>|
|<span data-ttu-id="eb593-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb593-115">Application</span></span>|<span data-ttu-id="eb593-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb593-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb593-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb593-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eb593-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb593-118">Request headers</span></span>
|<span data-ttu-id="eb593-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb593-119">Header</span></span>|<span data-ttu-id="eb593-120">値</span><span class="sxs-lookup"><span data-stu-id="eb593-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb593-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb593-121">Authorization</span></span>|<span data-ttu-id="eb593-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb593-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb593-123">承諾</span><span class="sxs-lookup"><span data-stu-id="eb593-123">Accept</span></span>|<span data-ttu-id="eb593-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb593-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb593-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb593-125">Request body</span></span>
<span data-ttu-id="eb593-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eb593-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb593-127">応答</span><span class="sxs-lookup"><span data-stu-id="eb593-127">Response</span></span>
<span data-ttu-id="eb593-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eb593-128">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb593-129">例</span><span class="sxs-lookup"><span data-stu-id="eb593-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb593-130">要求</span><span class="sxs-lookup"><span data-stu-id="eb593-130">Request</span></span>
<span data-ttu-id="eb593-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb593-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="eb593-132">応答</span><span class="sxs-lookup"><span data-stu-id="eb593-132">Response</span></span>
<span data-ttu-id="eb593-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eb593-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



