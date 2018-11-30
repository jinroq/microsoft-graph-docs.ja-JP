---
title: Delete deviceCategory
description: deviceCategory を削除します。
ms.openlocfilehash: a85190a47bca7ec58d899be3618ae59229ecef06
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024255"
---
# <a name="delete-devicecategory"></a><span data-ttu-id="81730-103">Delete deviceCategory</span><span class="sxs-lookup"><span data-stu-id="81730-103">Delete deviceCategory</span></span>

> <span data-ttu-id="81730-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81730-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81730-105">[deviceCategory](../resources/intune-shared-devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="81730-105">Deletes a [deviceCategory](../resources/intune-shared-devicecategory.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="81730-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="81730-106">Prerequisites</span></span>
<span data-ttu-id="81730-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81730-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81730-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81730-109">Permission type</span></span>|<span data-ttu-id="81730-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81730-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81730-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81730-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="81730-112">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="81730-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="81730-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="81730-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="81730-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81730-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81730-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81730-115">Not supported.</span></span>|
|<span data-ttu-id="81730-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81730-116">Application</span></span>|<span data-ttu-id="81730-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81730-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81730-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81730-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="81730-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81730-119">Request headers</span></span>
|<span data-ttu-id="81730-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81730-120">Header</span></span>|<span data-ttu-id="81730-121">値</span><span class="sxs-lookup"><span data-stu-id="81730-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81730-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81730-122">Authorization</span></span>|<span data-ttu-id="81730-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="81730-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81730-124">Accept</span><span class="sxs-lookup"><span data-stu-id="81730-124">Accept</span></span>|<span data-ttu-id="81730-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81730-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81730-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="81730-126">Request body</span></span>
<span data-ttu-id="81730-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="81730-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81730-128">応答</span><span class="sxs-lookup"><span data-stu-id="81730-128">Response</span></span>
<span data-ttu-id="81730-129">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="81730-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="81730-130">例</span><span class="sxs-lookup"><span data-stu-id="81730-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="81730-131">要求</span><span class="sxs-lookup"><span data-stu-id="81730-131">Request</span></span>
<span data-ttu-id="81730-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81730-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="81730-133">応答</span><span class="sxs-lookup"><span data-stu-id="81730-133">Response</span></span>
<span data-ttu-id="81730-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81730-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



