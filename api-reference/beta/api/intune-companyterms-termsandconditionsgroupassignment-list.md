---
title: リスト termsAndConditionsGroupAssignments
description: TermsAndConditionsGroupAssignment オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
ms.openlocfilehash: b37a75019e57d1ef4a5fb0a290f8bffba2e19fdc
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326811"
---
# <a name="list-termsandconditionsgroupassignments"></a><span data-ttu-id="a2dea-103">リスト termsAndConditionsGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="a2dea-103">List termsAndConditionsGroupAssignments</span></span>

> <span data-ttu-id="a2dea-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2dea-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2dea-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2dea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2dea-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2dea-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2dea-107">[TermsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a2dea-107">List properties and relationships of the [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2dea-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2dea-108">Prerequisites</span></span>
<span data-ttu-id="a2dea-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2dea-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2dea-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2dea-111">Permission type</span></span>|<span data-ttu-id="a2dea-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2dea-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2dea-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2dea-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2dea-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2dea-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a2dea-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2dea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2dea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2dea-116">Not supported.</span></span>|
|<span data-ttu-id="a2dea-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2dea-117">Application</span></span>|<span data-ttu-id="a2dea-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2dea-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2dea-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2dea-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a2dea-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2dea-120">Request headers</span></span>
|<span data-ttu-id="a2dea-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2dea-121">Header</span></span>|<span data-ttu-id="a2dea-122">値</span><span class="sxs-lookup"><span data-stu-id="a2dea-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2dea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2dea-123">Authorization</span></span>|<span data-ttu-id="a2dea-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a2dea-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2dea-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2dea-125">Accept</span></span>|<span data-ttu-id="a2dea-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2dea-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2dea-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2dea-127">Request body</span></span>
<span data-ttu-id="a2dea-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a2dea-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2dea-129">応答</span><span class="sxs-lookup"><span data-stu-id="a2dea-129">Response</span></span>
<span data-ttu-id="a2dea-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="a2dea-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2dea-131">例</span><span class="sxs-lookup"><span data-stu-id="a2dea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2dea-132">要求</span><span class="sxs-lookup"><span data-stu-id="a2dea-132">Request</span></span>
<span data-ttu-id="a2dea-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2dea-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

### <a name="response"></a><span data-ttu-id="a2dea-134">応答</span><span class="sxs-lookup"><span data-stu-id="a2dea-134">Response</span></span>
<span data-ttu-id="a2dea-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2dea-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 214

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
      "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
      "targetGroupId": "Target Group Id value"
    }
  ]
}
```





