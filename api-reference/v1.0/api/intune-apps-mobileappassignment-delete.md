---
title: Delete mobileAppAssignment
description: mobileAppAssignment を削除します。
author: tfitzmac
ms.openlocfilehash: 4cf58d159a260f3a31bb5a9e95ec698aaa6ccfc7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361685"
---
# <a name="delete-mobileappassignment"></a><span data-ttu-id="d8161-103">Delete mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="d8161-103">Delete mobileAppAssignment</span></span>

> <span data-ttu-id="d8161-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8161-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d8161-105">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d8161-105">Deletes a [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d8161-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8161-106">Prerequisites</span></span>
<span data-ttu-id="d8161-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8161-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8161-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8161-109">Permission type</span></span>|<span data-ttu-id="d8161-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8161-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8161-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8161-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d8161-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8161-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8161-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8161-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8161-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8161-114">Not supported.</span></span>|
|<span data-ttu-id="d8161-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8161-115">Application</span></span>|<span data-ttu-id="d8161-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8161-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8161-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8161-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d8161-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8161-118">Request headers</span></span>
|<span data-ttu-id="d8161-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8161-119">Header</span></span>|<span data-ttu-id="d8161-120">値</span><span class="sxs-lookup"><span data-stu-id="d8161-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8161-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8161-121">Authorization</span></span>|<span data-ttu-id="d8161-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d8161-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8161-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d8161-123">Accept</span></span>|<span data-ttu-id="d8161-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d8161-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8161-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8161-125">Request body</span></span>
<span data-ttu-id="d8161-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d8161-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8161-127">応答</span><span class="sxs-lookup"><span data-stu-id="d8161-127">Response</span></span>
<span data-ttu-id="d8161-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="d8161-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d8161-129">例</span><span class="sxs-lookup"><span data-stu-id="d8161-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d8161-130">要求</span><span class="sxs-lookup"><span data-stu-id="d8161-130">Request</span></span>
<span data-ttu-id="d8161-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8161-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d8161-132">応答</span><span class="sxs-lookup"><span data-stu-id="d8161-132">Response</span></span>
<span data-ttu-id="d8161-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8161-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



