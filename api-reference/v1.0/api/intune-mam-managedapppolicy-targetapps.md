---
title: targetApps アクション
description: まだ文書化されていません
ms.openlocfilehash: 532e928dace6f956cbe17865128e5831d845abf4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023023"
---
# <a name="targetapps-action"></a><span data-ttu-id="c8e0e-103">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="c8e0e-103">targetApps action</span></span>

> <span data-ttu-id="c8e0e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8e0e-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c8e0e-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8e0e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8e0e-106">Prerequisites</span></span>
<span data-ttu-id="c8e0e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8e0e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8e0e-109">Permission type</span></span>|<span data-ttu-id="c8e0e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8e0e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8e0e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8e0e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8e0e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8e0e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c8e0e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8e0e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8e0e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-114">Not supported.</span></span>|
|<span data-ttu-id="c8e0e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8e0e-115">Application</span></span>|<span data-ttu-id="c8e0e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8e0e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8e0e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="c8e0e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8e0e-118">Request headers</span></span>
|<span data-ttu-id="c8e0e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8e0e-119">Header</span></span>|<span data-ttu-id="c8e0e-120">値</span><span class="sxs-lookup"><span data-stu-id="c8e0e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8e0e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8e0e-121">Authorization</span></span>|<span data-ttu-id="c8e0e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8e0e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="c8e0e-123">Accept</span></span>|<span data-ttu-id="c8e0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8e0e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8e0e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8e0e-125">Request body</span></span>
<span data-ttu-id="c8e0e-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c8e0e-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c8e0e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8e0e-128">Property</span></span>|<span data-ttu-id="c8e0e-129">型</span><span class="sxs-lookup"><span data-stu-id="c8e0e-129">Type</span></span>|<span data-ttu-id="c8e0e-130">説明</span><span class="sxs-lookup"><span data-stu-id="c8e0e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8e0e-131">apps</span><span class="sxs-lookup"><span data-stu-id="c8e0e-131">apps</span></span>|<span data-ttu-id="c8e0e-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c8e0e-132">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="c8e0e-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c8e0e-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c8e0e-134">応答</span><span class="sxs-lookup"><span data-stu-id="c8e0e-134">Response</span></span>
<span data-ttu-id="c8e0e-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8e0e-136">例</span><span class="sxs-lookup"><span data-stu-id="c8e0e-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8e0e-137">要求</span><span class="sxs-lookup"><span data-stu-id="c8e0e-137">Request</span></span>
<span data-ttu-id="c8e0e-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c8e0e-139">応答</span><span class="sxs-lookup"><span data-stu-id="c8e0e-139">Response</span></span>
<span data-ttu-id="c8e0e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8e0e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```


