---
title: enrollmentConfigurationAssignments のリスト
description: enrollmentConfigurationAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 93ff52a8179409cc186decfc3e3cd4f627ca0002
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024120"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="36130-103">enrollmentConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="36130-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="36130-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="36130-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36130-105">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="36130-105">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36130-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="36130-106">Prerequisites</span></span>
<span data-ttu-id="36130-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="36130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36130-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="36130-109">Permission type</span></span>|<span data-ttu-id="36130-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="36130-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36130-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="36130-111">Delegated (work or school account)</span></span>|<span data-ttu-id="36130-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="36130-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="36130-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="36130-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36130-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36130-114">Not supported.</span></span>|
|<span data-ttu-id="36130-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="36130-115">Application</span></span>|<span data-ttu-id="36130-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="36130-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36130-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="36130-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="36130-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36130-118">Request headers</span></span>
|<span data-ttu-id="36130-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="36130-119">Header</span></span>|<span data-ttu-id="36130-120">値</span><span class="sxs-lookup"><span data-stu-id="36130-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36130-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="36130-121">Authorization</span></span>|<span data-ttu-id="36130-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="36130-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36130-123">承諾</span><span class="sxs-lookup"><span data-stu-id="36130-123">Accept</span></span>|<span data-ttu-id="36130-124">application/json</span><span class="sxs-lookup"><span data-stu-id="36130-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36130-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="36130-125">Request body</span></span>
<span data-ttu-id="36130-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="36130-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36130-127">応答</span><span class="sxs-lookup"><span data-stu-id="36130-127">Response</span></span>
<span data-ttu-id="36130-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="36130-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36130-129">例</span><span class="sxs-lookup"><span data-stu-id="36130-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="36130-130">要求</span><span class="sxs-lookup"><span data-stu-id="36130-130">Request</span></span>
<span data-ttu-id="36130-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="36130-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="36130-132">応答</span><span class="sxs-lookup"><span data-stu-id="36130-132">Response</span></span>
<span data-ttu-id="36130-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="36130-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



