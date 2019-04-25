---
title: enrollmentConfigurationAssignments のリスト
description: enrollmentConfigurationAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0741eb742cfa52f6461130a95ef9df834b2bf23e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32528653"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="b7d26-103">enrollmentConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="b7d26-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="b7d26-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7d26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7d26-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7d26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7d26-106">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b7d26-106">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7d26-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b7d26-107">Prerequisites</span></span>
<span data-ttu-id="b7d26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7d26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7d26-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7d26-110">Permission type</span></span>|<span data-ttu-id="b7d26-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7d26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7d26-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7d26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7d26-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7d26-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b7d26-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7d26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7d26-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7d26-115">Not supported.</span></span>|
|<span data-ttu-id="b7d26-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7d26-116">Application</span></span>|<span data-ttu-id="b7d26-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7d26-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7d26-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7d26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b7d26-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7d26-119">Request headers</span></span>
|<span data-ttu-id="b7d26-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7d26-120">Header</span></span>|<span data-ttu-id="b7d26-121">値</span><span class="sxs-lookup"><span data-stu-id="b7d26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7d26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7d26-122">Authorization</span></span>|<span data-ttu-id="b7d26-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7d26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7d26-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b7d26-124">Accept</span></span>|<span data-ttu-id="b7d26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7d26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7d26-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7d26-126">Request body</span></span>
<span data-ttu-id="b7d26-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b7d26-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7d26-128">応答</span><span class="sxs-lookup"><span data-stu-id="b7d26-128">Response</span></span>
<span data-ttu-id="b7d26-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b7d26-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7d26-130">例</span><span class="sxs-lookup"><span data-stu-id="b7d26-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7d26-131">要求</span><span class="sxs-lookup"><span data-stu-id="b7d26-131">Request</span></span>
<span data-ttu-id="b7d26-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7d26-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="b7d26-133">応答</span><span class="sxs-lookup"><span data-stu-id="b7d26-133">Response</span></span>
<span data-ttu-id="b7d26-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7d26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





