---
title: targetApps アクション
description: まだ文書化されていません
ms.openlocfilehash: 988410f4d96065151a7eb940e826979c455331da
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074473"
---
# <a name="targetapps-action"></a><span data-ttu-id="ef6f4-103">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="ef6f4-103">targetApps action</span></span>

> <span data-ttu-id="ef6f4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ef6f4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ef6f4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef6f4-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef6f4-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef6f4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ef6f4-108">Prerequisites</span></span>
<span data-ttu-id="ef6f4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef6f4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef6f4-111">Permission type</span></span>|<span data-ttu-id="ef6f4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef6f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef6f4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef6f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ef6f4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef6f4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef6f4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef6f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef6f4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-116">Not supported.</span></span>|
|<span data-ttu-id="ef6f4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef6f4-117">Application</span></span>|<span data-ttu-id="ef6f4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef6f4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef6f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}/targetApps
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="ef6f4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef6f4-120">Request headers</span></span>
|<span data-ttu-id="ef6f4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef6f4-121">Header</span></span>|<span data-ttu-id="ef6f4-122">値</span><span class="sxs-lookup"><span data-stu-id="ef6f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef6f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef6f4-123">Authorization</span></span>|<span data-ttu-id="ef6f4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef6f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ef6f4-125">Accept</span></span>|<span data-ttu-id="ef6f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ef6f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef6f4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef6f4-127">Request body</span></span>
<span data-ttu-id="ef6f4-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ef6f4-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ef6f4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef6f4-130">Property</span></span>|<span data-ttu-id="ef6f4-131">型</span><span class="sxs-lookup"><span data-stu-id="ef6f4-131">Type</span></span>|<span data-ttu-id="ef6f4-132">説明</span><span class="sxs-lookup"><span data-stu-id="ef6f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef6f4-133">apps</span><span class="sxs-lookup"><span data-stu-id="ef6f4-133">apps</span></span>|<span data-ttu-id="ef6f4-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ef6f4-134">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="ef6f4-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ef6f4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ef6f4-136">応答</span><span class="sxs-lookup"><span data-stu-id="ef6f4-136">Response</span></span>
<span data-ttu-id="ef6f4-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ef6f4-138">例</span><span class="sxs-lookup"><span data-stu-id="ef6f4-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef6f4-139">要求</span><span class="sxs-lookup"><span data-stu-id="ef6f4-139">Request</span></span>
<span data-ttu-id="ef6f4-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}/targetApps

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

### <a name="response"></a><span data-ttu-id="ef6f4-141">応答</span><span class="sxs-lookup"><span data-stu-id="ef6f4-141">Response</span></span>
<span data-ttu-id="ef6f4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef6f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





