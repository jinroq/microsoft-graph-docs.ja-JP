---
title: termsAndConditionsAssignments のリスト
description: termsAndConditionsAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1c9beea3297c1360ee11a1ed267a5d06e9247862
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962556"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="ff0d1-103">termsAndConditionsAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="ff0d1-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="ff0d1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff0d1-105">[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-105">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ff0d1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff0d1-106">Prerequisites</span></span>
<span data-ttu-id="ff0d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff0d1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff0d1-109">Permission type</span></span>|<span data-ttu-id="ff0d1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff0d1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff0d1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff0d1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ff0d1-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff0d1-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ff0d1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff0d1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff0d1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-114">Not supported.</span></span>|
|<span data-ttu-id="ff0d1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff0d1-115">Application</span></span>|<span data-ttu-id="ff0d1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff0d1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff0d1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ff0d1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff0d1-118">Request headers</span></span>
|<span data-ttu-id="ff0d1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff0d1-119">Header</span></span>|<span data-ttu-id="ff0d1-120">値</span><span class="sxs-lookup"><span data-stu-id="ff0d1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff0d1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff0d1-121">Authorization</span></span>|<span data-ttu-id="ff0d1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff0d1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ff0d1-123">Accept</span></span>|<span data-ttu-id="ff0d1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ff0d1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff0d1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff0d1-125">Request body</span></span>
<span data-ttu-id="ff0d1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff0d1-127">応答</span><span class="sxs-lookup"><span data-stu-id="ff0d1-127">Response</span></span>
<span data-ttu-id="ff0d1-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff0d1-129">例</span><span class="sxs-lookup"><span data-stu-id="ff0d1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff0d1-130">要求</span><span class="sxs-lookup"><span data-stu-id="ff0d1-130">Request</span></span>
<span data-ttu-id="ff0d1-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="ff0d1-132">応答</span><span class="sxs-lookup"><span data-stu-id="ff0d1-132">Response</span></span>
<span data-ttu-id="ff0d1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff0d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



