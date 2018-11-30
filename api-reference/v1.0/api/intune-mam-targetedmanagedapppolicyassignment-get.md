---
title: Get targetedManagedAppPolicyAssignment
description: targetedManagedAppPolicyAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 1d318a63f731fd3b28f2dd67a0e3c2ce8cff4740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021015"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="d7885-103">Get targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="d7885-103">Get targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="d7885-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7885-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7885-105">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d7885-105">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7885-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d7885-106">Prerequisites</span></span>
<span data-ttu-id="d7885-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7885-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7885-109">Permission type</span></span>|<span data-ttu-id="d7885-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7885-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7885-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7885-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d7885-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7885-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d7885-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7885-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7885-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7885-114">Not supported.</span></span>|
|<span data-ttu-id="d7885-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7885-115">Application</span></span>|<span data-ttu-id="d7885-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7885-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7885-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7885-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d7885-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d7885-118">Optional query parameters</span></span>
<span data-ttu-id="d7885-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d7885-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d7885-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7885-120">Request headers</span></span>
|<span data-ttu-id="d7885-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7885-121">Header</span></span>|<span data-ttu-id="d7885-122">値</span><span class="sxs-lookup"><span data-stu-id="d7885-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7885-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7885-123">Authorization</span></span>|<span data-ttu-id="d7885-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d7885-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7885-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7885-125">Accept</span></span>|<span data-ttu-id="d7885-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7885-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7885-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7885-127">Request body</span></span>
<span data-ttu-id="d7885-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d7885-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7885-129">応答</span><span class="sxs-lookup"><span data-stu-id="d7885-129">Response</span></span>
<span data-ttu-id="d7885-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d7885-130">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7885-131">例</span><span class="sxs-lookup"><span data-stu-id="d7885-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7885-132">要求</span><span class="sxs-lookup"><span data-stu-id="d7885-132">Request</span></span>
<span data-ttu-id="d7885-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7885-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d7885-134">応答</span><span class="sxs-lookup"><span data-stu-id="d7885-134">Response</span></span>
<span data-ttu-id="d7885-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7885-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 252

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



