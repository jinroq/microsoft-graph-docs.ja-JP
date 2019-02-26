---
title: Get enrollmentConfigurationAssignment
description: enrollmentConfigurationAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab7074722df42b187043de07b6a4524e97817a79
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262931"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="6c8a7-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6c8a7-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="6c8a7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c8a7-105">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-105">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c8a7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6c8a7-106">Prerequisites</span></span>
<span data-ttu-id="6c8a7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6c8a7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c8a7-109">Permission type</span></span>|<span data-ttu-id="6c8a7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c8a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c8a7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c8a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6c8a7-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c8a7-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6c8a7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c8a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c8a7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-114">Not supported.</span></span>|
|<span data-ttu-id="6c8a7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c8a7-115">Application</span></span>|<span data-ttu-id="6c8a7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c8a7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c8a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c8a7-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c8a7-118">Optional query parameters</span></span>
<span data-ttu-id="6c8a7-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c8a7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c8a7-120">Request headers</span></span>
|<span data-ttu-id="6c8a7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c8a7-121">Header</span></span>|<span data-ttu-id="6c8a7-122">値</span><span class="sxs-lookup"><span data-stu-id="6c8a7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c8a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c8a7-123">Authorization</span></span>|<span data-ttu-id="6c8a7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c8a7-125">承諾</span><span class="sxs-lookup"><span data-stu-id="6c8a7-125">Accept</span></span>|<span data-ttu-id="6c8a7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c8a7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c8a7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c8a7-127">Request body</span></span>
<span data-ttu-id="6c8a7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c8a7-129">応答</span><span class="sxs-lookup"><span data-stu-id="6c8a7-129">Response</span></span>
<span data-ttu-id="6c8a7-130">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-130">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c8a7-131">例</span><span class="sxs-lookup"><span data-stu-id="6c8a7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c8a7-132">要求</span><span class="sxs-lookup"><span data-stu-id="6c8a7-132">Request</span></span>
<span data-ttu-id="6c8a7-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6c8a7-134">応答</span><span class="sxs-lookup"><span data-stu-id="6c8a7-134">Response</span></span>
<span data-ttu-id="6c8a7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c8a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "value": {
    "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
    "id": "705b021c-021c-705b-1c02-5b701c025b70",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



