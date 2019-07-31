---
title: Get enrollmentConfigurationAssignment
description: enrollmentConfigurationAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 58f96d6303d84b194223ce8fb5c281a63bef68d2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994055"
---
# <a name="get-enrollmentconfigurationassignment"></a><span data-ttu-id="ace0c-103">Get enrollmentConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ace0c-103">Get enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="ace0c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ace0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ace0c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ace0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ace0c-106">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ace0c-106">Read properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ace0c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ace0c-107">Prerequisites</span></span>
<span data-ttu-id="ace0c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ace0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace0c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ace0c-110">Permission type</span></span>|<span data-ttu-id="ace0c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ace0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ace0c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ace0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ace0c-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ace0c-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ace0c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ace0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ace0c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ace0c-115">Not supported.</span></span>|
|<span data-ttu-id="ace0c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ace0c-116">Application</span></span>|<span data-ttu-id="ace0c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ace0c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ace0c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ace0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ace0c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ace0c-119">Optional query parameters</span></span>
<span data-ttu-id="ace0c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ace0c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ace0c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ace0c-121">Request headers</span></span>
|<span data-ttu-id="ace0c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ace0c-122">Header</span></span>|<span data-ttu-id="ace0c-123">値</span><span class="sxs-lookup"><span data-stu-id="ace0c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ace0c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ace0c-124">Authorization</span></span>|<span data-ttu-id="ace0c-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ace0c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ace0c-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ace0c-126">Accept</span></span>|<span data-ttu-id="ace0c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ace0c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ace0c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ace0c-128">Request body</span></span>
<span data-ttu-id="ace0c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ace0c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ace0c-130">応答</span><span class="sxs-lookup"><span data-stu-id="ace0c-130">Response</span></span>
<span data-ttu-id="ace0c-131">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ace0c-131">If successful, this method returns a `200 OK` response code and [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ace0c-132">例</span><span class="sxs-lookup"><span data-stu-id="ace0c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ace0c-133">要求</span><span class="sxs-lookup"><span data-stu-id="ace0c-133">Request</span></span>
<span data-ttu-id="ace0c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ace0c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="ace0c-135">応答</span><span class="sxs-lookup"><span data-stu-id="ace0c-135">Response</span></span>
<span data-ttu-id="ace0c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ace0c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





